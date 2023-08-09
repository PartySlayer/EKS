# EKS
Phase 2 of the Infrastructure Automation project

In this phase I'm going to start preparing the enviroment to deploy a spring boot application.

After accessing a fresh EC2, I started updating.
I then cURL'd aws-cli.zip file, unzipped it and installed it.
![aws-cli](https://github.com/PartySlayer/EKS/assets/120326157/1ff72227-668e-4378-ad26-9985e2b8610a)

It was now time to configure it but before that, I had to create the Access Key ID and AWS Secret Access Key.
![aws-cli1](https://github.com/PartySlayer/EKS/assets/120326157/3855b128-4607-4c90-9084-5216db8828cd)

Configuration ended.
![aws-cli2](https://github.com/PartySlayer/EKS/assets/120326157/9e69e6e0-9745-44d6-b261-e6be62603f8e)


I then downloaded Kubectl, made it executable and copied its directory in the PATH variable.
It's a binary so this is mandatory in order to execute it correctly.
![kubectl](https://github.com/PartySlayer/EKS/assets/120326157/94ea605a-b455-4f82-bd11-95e4c7d39be0)

Kubectl installed correctly.

I needed to create an IAM role to allow aws resources management from Kubernetes control plane.
![IAM](https://github.com/PartySlayer/EKS/assets/120326157/292ca801-0bab-4330-bcc8-ea37826ae5a6)

At this point I could create a new cluster.
![cluster](https://github.com/PartySlayer/EKS/assets/120326157/46db2306-772d-4a00-a7ea-dc0f0df8fb4a)

I configured it using previously created network settings.
![EKS](https://github.com/PartySlayer/EKS/assets/120326157/eae84a4d-b2fa-432b-aeb6-e6d6616e021e)

After around 20 minutes, the cluster was finally active.
![custer1](https://github.com/PartySlayer/EKS/assets/120326157/9566e5a9-b438-408e-9f7e-49cc4d5042b7)

Then I created a Node IAM role...
![nodeIAM](https://github.com/PartySlayer/EKS/assets/120326157/ea58d1d7-5dd7-425d-b451-cfceeacaa6e7)

...so I could configure the worker node.
![nodeworker](https://github.com/PartySlayer/EKS/assets/120326157/b3c2436a-0e26-41f5-b031-c9b566500d59)


It was time to make kubectl use the cluster.
![nodeworker1](https://github.com/PartySlayer/EKS/assets/120326157/5893db6a-492f-42a1-b6aa-e65b161383fc)


Finally, everything was up and running!
![nodeworker2](https://github.com/PartySlayer/EKS/assets/120326157/1bc1d87f-573b-45ed-b159-d99db8659ae2)

