

# ECR-Deployer


A simple docker in docker image pre-configured with the tools necessary to push images to [AWS ECR](https://aws.amazon.com/en/ecr/ "AWS ECR"). Intended to be used in CI/CD pipelines.

# How to use
- Pull the image with the command `docker pull itsadeadh2/ecr-deployer`
- Define the both `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` envvars to your corresponding[ iam user credentials](https://aws.amazon.com/iam/ " iam user credentials") 
with `docker run -it -e AWS_ACCESS_KEY=YOURACCESSKEY -e AWS_SECRET_ACCESS_KEY=YOURSECRET itsadeadh2/ecr-deployer sh`
After that you can execute commands like `aws ecr get-login` without problems.