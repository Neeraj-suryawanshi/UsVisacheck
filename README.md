# UsVisacheck


#git commands
git add .
git commit -m "commitmessage"
git push origin main 

Creating envirornment:

conda create -n usvisa python=3.8 y
coda acivate usvisa
"""
__init__ we are using because every file we can take as local pacakge and use internally by importing from one folder to another folder

we can call import our custom function:

from us_visa.components.data_transformation import nrj
nrj()

"""

### Git command 

git add .

git commit -m "Updated"

git push origin main

### How to run?
conda create -n visa python=3.8 -y
conda activate visa
pip install -r requirements.txt

# Workflow
1.constant
2.config_entity
3.artifact_entity
4.component
5.pipeline
6.app.py


# Export the environment variable
run below command in git bash
export MONGODB_URL="mongodb+srv://suryawanshineeraj32:ULWtnlxyLwQ7advn@cluster0.ab2a2z2.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0"
format (export MONGODB_URL="mongodb+srv://<username>:<password>....")

# we can set environment variable directly also 

### Export the environment variable
#export MONGODB_URL="mongodb+srv://<username>:<password>...."

export AWS_ACCESS_KEY_ID=""

export AWS_SECRET_ACCESS_KEY=""


### steps for deployment
# 1 Login to AWS console.

# 2 Create IAM user for deployment
#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess

# 3 Create ECR repo to store/save docker image
- Save the URI: 136566696263.dkr.ecr.us-east-1.amazonaws.com/mlproject

# 4 Create EC2 machine (Ubuntu)
# 5 Open EC2 and Install docker in EC2 Machine:

#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

# 6 Configure EC2 as self-hosted runner:
setting>actions>runner>new self hosted runner> choose os> then run command one by one

# 7  Setup github secrets:














