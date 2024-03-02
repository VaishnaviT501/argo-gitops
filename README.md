**DevOps Internship Assignment Documentation**

**Introduction**
The purpose of this documentation is to provide a comprehensive overview of the DevOps Internship Assignment attempted by Vaishnavi Tiwari. This assignment focused on hands-on experience with GitOps practices, utilizing Argo CD for continuous deployment and Argo Rollouts for advanced deployment strategies within a Kubernetes environment.

**Assignment Overview**
The assignment aimed to dockerize a simple web application, deploy it to a Kubernetes cluster using Argo CD, and manage its release process with Argo Rollouts. It consisted of three main tasks:

**Task 1: Setup and Configuration**
In the initial phase of the assignment, the focus was on establishing the groundwork for the GitOps pipeline. This involved setting up the necessary infrastructure and configurations. 
•	Created a GitHub repository to host the source code.
To begin, a GitHub repository was created to serve as the central repository for hosting the source code of the web application. 
•	Installed Argo CD on the Kubernetes cluster following the official documentation.
•	Installed the Argo Rollouts controller in the Kubernetes cluster according to the official guide.

**Task 2: Creating the GitOps Pipeline**
•	Dockerized the simple web application and pushed it to a public container registry.
This involved creating a Docker image for the application and ensuring it could run in a containerized environment.
I started by creating a Dockerfile, which is a set of instructions used by Docker to build the Docker image. This file includes details like the base image, copying application files, exposing ports, and defining the command to run the application. I used basic “nginx” image with a tag named “latest”.
By incorporating Visual Studio Code as the development environment and orchestrating the Docker CLI commands for image construction, the Dockerization process of the application was seamlessly integrated into the development workflow.
•	Modified Kubernetes manifests in the forked repository to use the Docker image.
Following the successful creation of the Docker image, I made modifications to the Kubernetes deployment and service manifests in the GitHub repository which can be reviewed in “deployment.yml”. These modifications ensured that the Kubernetes resources, such as Deployments and Services, were configured to use the Docker image pushed to the container registry.
•	Configured Argo CD to monitor the repository and automatically deploy changes to the Kubernetes cluster.

**Task 3: Implementing a Canary Release with Argo Rollouts**
•	Defined a rollout strategy using Argo Rollouts, specifying a canary release strategy.
•	Despite attempting to monitor the rollout using Argo Rollouts CLI and Kubernetes dashboard, I was unable to progress beyond the setup stage due to insufficient understanding of the process and configurations.

**Challenges:**
•	Limited Understanding of Argo Rollouts:
Lack of familiarity with Argo Rollouts and specific configurations for canary releases. Attempted implementation based on available knowledge but faced difficulties due to insufficient prior experience and detailed documentation.
•	Complexity of Canary Release Strategies:
Canary releases demand meticulous planning and configuration adjustments for safe deployment. Grappled with the intricacies of defining canary steps and monitoring the rollout process, acknowledging the complexity associated with these strategies.

**Solutions:**
•	I adopted a trial-and-error approach to identify and fix build failures. 
•	I read the documentation and searched some solutions on Youtube and Google to help me understand Argo CD and Argo Rollout.

**Conclusion:**
The DevOps Internship Assignment provided valuable hands-on experience with GitOps practices, Argo CD, and Argo Rollouts within a Kubernetes environment. This assignment helped me enhance my skills in continuous deployment, release management, and documentation, contributing to the professional growth and development.

