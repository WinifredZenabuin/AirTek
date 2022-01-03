
# AirTek
This infrastructure is a production quality infrastructure provisioned on AWS Platform

Before you start, please do the following:
•	Make sure you create an S3 Bucket on AWS to lock the state file, and customise the code accordingly with the region and your profile credentials
•	Deploy vpc_module (to get the VPC Network infrastructure). The state file will locked in the S3 bucket you created above
•	Then deploy ec2_public_module (to get the servers deployed in the vpc accordingly)
•	After the deployment, the application was tested and a weather reading was received on the  web browser


The Following point should be considered when implementing security on AWS VPC
•	Use multiple Availability Zone deployments so you have high availability.
•	Use Load balancers to manage traffic
•	Use Multi-AZ (Sync Replication) for DB)
•	Use security groups and network ACLs.
•	Use IAM policies to control access.
•	Use Amazon CloudWatch to monitor your VPC components and VPN connections.
•	Use flow logs to capture information about IP traffic going to and from network interfaces in your VPC. 
