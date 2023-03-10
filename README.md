# **Information regarding the deployed application**
This project was part of the Advanced Web Development Nanodegree, it was about deploying a provided full-stack application on AWS services:
*	Backend on Elastic Beanstalk (EB)
*	Frontend on Simple Storage Service (S3)
*	Postgres database on Relational Database System (RDS)

And the other part was integrating Circle-CI pipeline with GitHub source code for continuous integration and continuous delivery which automatically deployed to AWS whenever the project had a commit on certain branch.


## [Udagram live](http://khalifa-udagram-bucket.s3-website-us-east-1.amazonaws.com/)
## [Screenshots of services and their healths](/documentation/screenshots/)
## Diagrams
### [AWS architecture](/documentation/architecture%20diagrams/Architecture.jpg)
### [Deployment pipeline](/documentation/architecture%20diagrams/pipeline.jpg)
## Documentations

### [App dependencies](/documentation/App%20dependencies.md)
### [Infrastructure description](/documentation/Infrastructure%20description.md)

### [Pipeline process](/documentation/Pipeline%20process.md)

<br><br/>
# **Hosting a Full-Stack Application**

### **You can use you own project completed in previous courses or use the provided Udagram app for completing this final project.**

---

In this project you will learn how to take a newly developed Full-Stack application built for a retailer and deploy it to a cloud service provider so that it is available to customers. You will use the aws console to start and configure the services the application needs such as a database to store product information and a web server allowing the site to be discovered by potential customers. You will modify your package.json scripts and replace hard coded secrets with environment variables in your code.

After the initial setup, you will learn to interact with the services you started on aws and will deploy manually the application a first time to it. As you get more familiar with the services and interact with them through a CLI, you will gradually understand all the moving parts.

You will then register for a free account on CircleCi and connect your Github account to it. Based on the manual steps used to deploy the app, you will write a config.yml file that will make the process reproducible in CircleCi. You will set up the process to be executed automatically based when code is pushed on the main Github branch.

The project will also include writing documentation and runbooks covering the operations of the deployment process. Those runbooks will serve as a way to communicate with future developers and anybody involved in diagnosing outages of the Full-Stack application.

# Udagram

This application is a simple cloud application developed alongside the Udacity Cloud Developer Nanodegree program. It allows users to register and log into a web client, post photos to the feed, and process photos using the Machine Learning Microservice.



### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing
1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

