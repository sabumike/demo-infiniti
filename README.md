# demo-infiniti
Cloudformation demo for Infiniti

The cloudformation script creates the two ec2 instances with apache as the webserver to display the content. These ec2 instances are open to both ports 80 and 22 with necessary security groups. 

## Region:

Region selected on AWS: **Oregon**

## Configuration Items:
Following configuration items  (Value) can be modified in the cloudformation scripts as required. These values are hardcoded in the scripts so that the configuration items can be preserved and tracked.

**Change the keypair before running the script**

				"GeneralName": {"Value": "demo"},
				"EnvName": {"Value": "demo"},
				"KeyName": {"Value":"infiniti-keypair"}, 
				"RegionAZNameA": {"Value":"us-west-2a"},
				"RegionAZNameC": {"Value":"us-west-2c"},
				"VPCName": {"Value":"Demo VPC"},
				"VpcCidrBlock": {"Value":"10.0.0.0/24"},
				"PublicCidrA": {"Value":"10.0.0.0/27"},
				"PublicCidrC": {"Value":"10.0.0.64/27"},
				"ImageID": {"Value":"ami-b04e92d0"},
				"InstanceType": {"Value":"t2.micro"}
        
## Run the scripts
- the script can be run in AWS console under Cloudformation services. (or) 
- the script can be run in a AWS command line with the following syntax.




