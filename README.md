# Lab-Managing-Resources-with-Tagging
## This lab is divided into two parts:
•	In the Task portion of this lab, you will use the AWS Command Line Interface (CLI) to inspect the tags assigned to a number of Amazon EC2 instances. You will then use pre-provided scripts to shut down and start up a number of Amazon EC2 instances simultaneously, based on their tags.
•	In the Challenge portion of this lab, you will be challenged to think of a way to terminate instances that fail to implement specific tags.
Objectives After completing this lab, you will be able to:
•	Apply tags to existing AWS resources.
•	Find resources based on tags.
•	Use the AWS CLI or AWS SDK for PHP to stop and terminate Amazon EC2 instances based on certain attributes of the resource.
Duration
This lab will require approximately 45 minutes to complete.
Scenario
The environment for this lab (pictured below) consists of:
•	Amazon VPC named Lab VPC
•	Public subnet
•	Private subnet
•	Amazon EC2 Linux instance named CommandHost [AWS Command Line Interface (CLI) tools have been pre-installed and configured for you on this instance]
•	8 Amazon EC2 Linux instances
•	Private instances have three custom tags applied to them:
Tag Name	content
Project	The project that the instance belongs to. The instances in this lab belong to one of two projects: ERPSystem and Experiment1.
Version	The version of the project that this instance belongs to. All Version tags are currently set to 1.0.
Environment	One of three values: development, staging, or production.


In the Task portion of this lab, you will log in to the Command Host and run some commands to find and change the Version tag on all development instances. You will run several examples that show how you can use the JMESPath syntax supported by the AWS CLI --query option to return richly formatted output. You will then use a set of pre-provided scripts to stop and re-start all instances that are tagged as belonging to the development environment.
![image](https://github.com/Tomtwiny121/Lab---Managing-Resources-with-Tagging/assets/128513453/29e94d6d-9c84-401e-93ce-7c37ae7ee1ed)
