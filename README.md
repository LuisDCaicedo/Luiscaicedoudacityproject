# udacityproject

For This Project I created the Diagram in this folder to show how i built my infrastructure

I created 4 Subnets Within my VPC 2 Public to Private 
An internet gateway was also added to allow traffic to go outside of our VPC
2 Natgateways were created in the public subnets in each AZ with an attached Elastic IP on each to allow high availabilty. 
Routes and RouteTables were also created allowing traffic to properly be routed within our services. 
An Application load balancer with a Listener was added to help properly distrubute traffic load in our application. 
In our private subnets an Autoscaling group was created with a launch configuration to help spin up our application in two AZ's to allow for high availability. 
The webservers in our Private Subnet were put in Webserver Security group. 

The webservers Assume an IAM role to get accesss to an S3 bucket that has our Application code. 


O
