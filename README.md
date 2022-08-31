# FluxOps
GitOps with Flux


Flux Edge computing

A way of implementing Continuous Deployment for Imagine Cloud native applications. It focuses on a developer-centric experience when operating infrastructure, by using tools developers are already familiar with, including Git and Continuous Deployment tools_, this means that GitOps helps you with your continuous deployment in general.



-   **Infrastructure as a code**: This refers to a declarative way to provide infrastructure or deployments for your applications
-   **Merge requests or pull requests**: A way to manage infrastructure or application code updates across multiple changes and collaborators. Source code management systems like Git enable merge or pull-request based workflows and a mechanism to manage this, usually using a Git repository. In this way, a team can have an approval and review mechanism to apply changes
-   **CI/CD**: Continuous Integration and Continuous Delivery includes by nature, all the process of building, checking, and deploying applications and changes to those software applications. GitOps is used to automate the continuous deployment for a cloud native application.

In this chapter, you will find tools that provide mechanisms for CI/CD automation pipelines. Let’s pay attention to the following diagram that shows a summary of how a GitOps works:



GitOps outlined processes as depicted in the diagram:

-   **Commit code to the source**: First, Here a developer makes changes and pushes their changes to a source or repository, for example, a git repository hosted at GitHub.
-   **Sync changes**: A GitOps tool, like for example Flux, periodically detects changes in the source.
-   **Provision or reconcile changes**: Once the GitOps tool detects changes, it aims this could automate to the process of update a deployment based on the declarative configuration changes found. The tool triggers This could include processes to modify as changing configurations, update the container image for an application using containers, and so on. Sometimes if the resource or deployment doesn’t exist, you have to provision the resources or reconcile comparing changes. This means that a GitOps tool regularly works with declarative definitions to reflect the state of your infrastructure or application.

Finally, the user will see the changes accessing their application, and you can also add some additional processes like notification if a process was finalized, or an alert, if something fails.

In general, this is how a GitOps process works Flux as our GitOps tool, to implement GitOps processes to automate our applications deployments and updates.

## GitOps principles

There are some principles that you have to follow if you are using GitOps to automate your continuous deployments, based on Weave works, these principles are:

-   Declarative definitions: You can often find these definitions using YAML files, but they could also be found in other formats as JSON and so on.
-   State of your applications versioned with Git: GitOps tools, use git repositories to store changes and states for applications
-   Approve changes that can be applied automatically to your resources: Git repository or services provide ways to automate a trigger tool when some changes or merges are detected
-   Software agents listening to changes notifying or alerting: GitOps tools also have daemons listening to changes a ready to launch action like —changing a repository with new image tag in case of applications using containers.

## GitOps benefits

Now you know how a GitOps tool works and how GitOps process helps you to automate your continuous deployment, now it's time to know GitOps benefits.

The benefits of GitOps based on Weave Works are:

-   **Increase productivity**: An automated process speed execution time, in this case more changes and updates for your applications in less time
-   **Enhanced developer experience**: GitOps tools, usually launch automated processes on your git repository, and this will be launched automatically without knowing the internal of the processes, for example, for applications using Kubernetes, a developer doesn’t have to know Kubernetes in some cases. But the depends on how your application is structured.
-   **Improved stability**: Logs of GitOps tools are included by default, this helps to meet some security and monitoring features.
-   **Higher reliability**: GitOps tools give you the ability to implement rollback mechanisms, reducing downtime for your applications if a change has an impact on the operation of your system.
-   **Consistency and standardization**: GitOps tools have structures to define your applications, and gives you best practices for your applications definitions, pipelines, or updates.
-   **Stronger security guarantees**: GitOps tools have security features like cryptography for secrets, track and manage changes, this brings you the path to secure your applications.

Now let’s move on to understand how GitOps works in a Cloud Native context.

## GitOps, Cloud Native, and Edge Computing

As we know, cloud native refers to the use of applications using technologies such as containers, microservices, CI/CD in the context of a DevOps culture. So, you can find an intersection for this concept when a GitOps tool is designed to run on cloud native environments, for example Kubernetes clusters.

A GitOps tool can help you to automate the continuous deployment process for your Kubernetes applications. There are tools like Argo CD or Flux that can help you to implement GitOps for your applications.

Application focus running low resources environments using ARM processors, in this case, Flux has support for ARM while Argo CD doesn’t. This chapter focuses on implementing GitOps with Flux using ARM devices. 
