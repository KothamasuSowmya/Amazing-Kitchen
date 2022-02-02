# Build for 
# Automate-For-Good hackathon 
check it out :- https://devpost.com/software/automate-configuration 
## Amazing-Kitchen
## Inspiration

Doing configuration need an extra time and effort. You can use chef to configure the Operating System with cookbooks. 
Is possible to automate another level ? The answer of the question yes. 

## What it does

we created a platform to do configuration with few clicks. It's called Amazing Kitchen. Amazing Kitchen will do the configuration in any Operating System from Graphical User Interface 

- **How to Configure**

![Configure](https://drive.google.com/uc?export=view&id=1P-Ml90WKWVedzp2Dawa4UlFmAAZhiVAa)

1. Browse to [Amazing Kitchen](https://tinyurl.com/amazing-kitchen)
2. Navigate to Configuration page 
3. Click on the configure button at the end of the page
4. Provide the required details
5. Amazing Kitchen will configure your Operating System

## How we built it

***Team Formation***

The primary step of this project is the same as any other project we formed as a team and we called ourselves ***Clever Cooks***. Team members are from all over India. we are connected over LinkedIn and connected with referrals of friends. The team is a combo of multiple skilled people. So, we divided work

- **User Interface and Experience**

Sowmya worked on website development. She created code for the website and the website is informative and has multiple details about Amazing Kitchen.

- **Backend**

Sridhar worked as a Full Stack Developer. Setup chef server, Written cookbooks for the project. Integrated frontend and backend. Made 

- **DevOps**

Siva Naik worked on the creation of the pipeline with Frontend and Backend and automated from Development to Production with DevOps tools: Docker, Kubernetes, Git Hub Actions, ArgoCD, Terraform, and Cloud Platforms: Microsoft Azure for AKS

***Pipeline***
![Architecture](https://drive.google.com/uc?export=view&id=1VD0JhqGHkLfhXEuuPQoN8RvRLucEBnGQ)

- The Architecture team/DevOps team has already pushed the GitHub Actions' code in .git/workflows/ directory in both the repositories. For every event of code change, the GitHub Actions will trigger and build a Docker Image and save the image in Docker Hub. The Docker hub credentials are passed from GitHub repository secrets

- The repositories also have the Helm charts uploaded by the DevOps team in the manifests directory to deploy the application with ArgoCD running on AKS

- The AKS Cluster is already provisioned and the ArgoCD Helm chart is deployed on top of AKS with Terraform, Infrastructure as a Code tool

- The DevOps team is doing operations from the Azure cloud shell. They created two ArgoCD projects with declarative manifests the projects will monitor those two repositories for code change and deploy on top AKS when they sync the repositories

## Challenges we ran into

We faced a ton of challenges throughout the project :

- Integration of multiple DevOps tools in the complete pipeline
- Finding the correct hyperparameters when training the Model
- Making the website responsive
- To secure the credentials for the client server to do configuration.

## Accomplishments that we're proud of

- Integrated 10+ tools to automate everything from development to production
- The Website is designed in such a way it is very user-friendly and simple to navigate
- The predictions are almost correct.
- We implemented the project in 3 days before the deadline of the Hackathon

## What we learned

We understood the power of integrating multiple tools and technologies and solving real-world problems using them. Also as we worked in a team we learned how to work in a team.

## What's next for Amazing Kitchen

- Add some security features to save the pem file with us
- Make it production ready to deliver to customers

## References & Further Readings

- [Chef](https://learn.chef.io/)
- [Azure](https://docs.microsoft.com/en-us/azure/?product=featured)
- [AWS](https://docs.aws.amazon.com/)
- [Flask](https://flask.palletsprojects.com/en/2.0.x/)
- [Helm](https://helm.sh/docs/)
- [GitHub Actions](https://docs.github.com/en/actions)
- [Docker](https://docs.docker.com/)
- [Dockerfile](https://docs.docker.com/engine/reference/builder/)
- [Kubernetes](https://kubernetes.io/docs/home/)
- [ArgoCD](https://argoproj.github.io/argo-cd/)
- [Terraform](https://www.terraform.io/docs/index.html)
# Amazing-Kitchen
