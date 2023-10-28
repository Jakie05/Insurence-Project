# DevOps Certification Project - Insurance Domain Web Application

This project is designed to help you gain hands-on experience in implementing a CI/CD pipeline and automation for an Insurance Domain Web Application. The project involves the development of a microservice with front-end (HTML, CSS, AngularJS) and back-end (Java Spring Boot) components. The application runs on port 8081.

## Project Overview

- **Company**: Insure Me, a global leading insurance provider based in the USA.
- **Initial Architecture**: The company initially used a monolithic application architecture.
- **Challenges**: Faced difficulties in managing application infrastructure, deployments, and the need for frequent product updates.
- **Solution**: Transform monolithic architecture into a microservices-based architecture and implement DevOps practices using AWS as the primary cloud service provider.

## Microservice Development

### Front-end (HTML, CSS, AngularJS):

1. Clone the project repository to your local machine:


2. Front-End (HTML, CSS, AngularJS):
- Navigate to the front-end directory in your project folder.
- Install the required dependencies:

  ```
  npm install
  ```

- Start the front-end development server on port 8081:

  ```
  ng serve --port 8081
  ```

- The front-end will be accessible at http://localhost:8081 in your web browser.

### Back-end (Java Spring Boot):

1. Open the project in your Java Spring Boot-compatible IDE.

2. Locate the `application.properties` or `application.yml` configuration file.

3. Set the server port to 8081:


4. Run the Spring Boot application from your IDE or using the command-line interface:


5. The back-end API will be accessible at http://localhost:8081.

## API Endpoints

The application provides the following API endpoints:
- POST /createPolicy
- PUT /updatePolicy/{policy id}
- GET /viewPolicy/{policy id}
- DELETE /deletePolicy/{policy id}

These endpoints are used to manage insurance policies in the system.

## CI/CD Implementation

To implement a CI/CD pipeline and automation flow, follow these steps:

1. **Version Control with Git**:
- Set up a Git repository to host your project code.
- Clone the repository to your local development environment using Git.

2. **Microservice Development**:
- Develop a Mavenized microservice using Spring Boot with an in-memory H2 database.
- Create the API endpoints mentioned in the project description.
- Write necessary JUnit test cases.
- Generate HTML reports using TestNG.
- Push the code to your GitHub repository.

3. **Setting Up Jenkins for CI/CD**:
- Install Jenkins on a server or virtual machine.
- Configure Jenkins with the necessary plugins, including Git integration, TestNG, Docker, and AWS.
- Create a Jenkins job to build and test your microservice. Configure it to fetch code from your Git repository.
- Configure a GitHub Webhook to trigger the Jenkins job when changes are pushed to the master branch.

4. **Docker Containerization**:
- Create a Dockerfile to package your microservice as a Docker container.
- Build a Docker image of your microservice using Jenkins.
- Push the Docker image to a Docker registry (e.g., Docker Hub).

5. **Ansible for Configuration Management**:
- Install and configure Ansible on a server that can manage your deployment infrastructure.
- Write Ansible playbooks to automate the configuration and provisioning of your servers in AWS.

6. **Selenium Test Automation**:
- Develop Selenium tests to automate the testing of your web application.
- Configure Jenkins to run Selenium tests as part of the CI/CD pipeline.

7. **AWS for Deployment**:
- Set up an AWS environment by creating an AWS account and the necessary resources, including EC2 instances to serve as your deployment servers.
- Secure access to AWS resources using security groups, IAM roles, and user access.
- Use Ansible to automate the deployment of your Dockerized microservice to AWS EC2 instances.

8. **Automating the Flow**:
- When developers push code to the GIT master branch, a GitHub Webhook triggers your Jenkins job.
- Jenkins checks out the latest code, builds the microservice, runs JUnit tests, and generates test reports.
- Jenkins builds a Docker image of your microservice and pushes it to a Docker registry.
- Ansible is triggered to provision and configure your AWS EC2 instances for deployment.
- Jenkins runs Selenium tests to verify the deployed application.
- If all tests pass, Jenkins deploys the application to the production server in AWS.

9. **Monitoring and Logging (Optional)**:
- Implement monitoring and logging solutions (e.g., ELK Stack, Prometheus, Grafana) to track the performance and health of your microservices.

10. **Documentation**:
 - Create documentation for the entire CI/CD pipeline, including setup instructions and API documentation.

11. **Testing and Validation**:
 - Test the entire CI/CD pipeline and automation flow thoroughly to ensure that it works as expected.

## Insurance Domain Knowledge

To gain a deeper understanding of the insurance domain and the specific requirements of this project, please refer to the "Insurance-domain.pdf" document included in the project. This document contains information about the insurance-related functionalities, policies, and use cases that your application should support.

Thank you for using the Insurance Domain Web Application and exploring the world of DevOps and CI/CD.
