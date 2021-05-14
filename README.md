# Di_Data CI/CD Pipeline..!!
# Using AWS Elastic Beanstalk, AWS CodeBuilt, AWS CodePipeline
# To deploy a Node.js Sample App

This repository contains a sample Node.js web application built using [Express](https://expressjs.com/), to be used in Di_Data CI/CD Pipeline..!!

# Prerequisites:-

○ A Github account
○ A sample application to be deployed
○ AWS Elastic Beanstalk
○ AWS CodeBuild
○ AWS CodePipeline

# Github

Create a code repository containing a simple Node.js web app to trigger a continuous delivery pipeline

# AWS Elastic Beanstalk

Create and deploy a web application using AWS Elastic Beanstalk environment

# Built Project

Use AWS CodeBuild to build the source code stored in our GitHub repository

# -> Buildspec File

version: 0.2
phases:
    build:
        commands:
            - npm i --save
artifacts:
    files:
        - '**/*'
	
# Create CI/CD Pipeline

Set up a continuous delivery pipeline using AWS CodePipeline to configure a source stage using GitHub repo
Configure a build stage using AWS CodeBuild
Configure a deploy stage using AWS ElasticBeanstalk application
Then deploy the application hosted on GitHub to ElasticBeanstalk through a pipeline which will allows developers to release software more quickly by automating the build, test and deploy processes.



# Instructions to execute and test the solution..!!

1. Navigate to the Github Repo:-

Link:https://github.com/jdiph051/aws-elastic-beanstalk-express-js-sample

2. Open apps.js file and edit the code in line 5  

3. Commit the code (CodePipeline will automatically trigger CodeBuild and deploy changes committed)

4. Open deployed web application

Link: didatadevopsgettingstarted-env.eba-mbiyhaci.us-east-2.elasticbeanstalk.com

5. New changes should be displayed in less than 3min after the code has been committed

6. Repeat steps 2 through 3 to see continues integration

