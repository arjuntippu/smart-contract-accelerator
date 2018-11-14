# Deploy OFS SmartContract Accelarator in AWS with one click

ObjectFrontier Smart Contract Accelerator is a click button Blockchain solution that installs a private Ethereum blockchain instance in your AWS environment. It comes pre-packeged with an Admin DApp that you can use to:

- Configure your private network
- Compile and deploy solidity-based smart contracts
- Create new application experiences
- View each block in the chain
- OFS Blockchain provisions a default master account and preloads private tokens to get you started with developing your blockchain applications and smart contracts.

After you intall. Launch the app, login to admin interface using the creds admin/admin.

## Pre-requisite for the AWS deployment
- Active AWS account .  
    - Link to create account - <a href="https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/" target="_blank">Click here</a> 
- Key pair if you want to SSH to EC2 Instance . 
    - Link to create Key pair - <a href="https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html" target="_blank"> Click here</a>
    
## One click deployment AWS Buttons

| Buttons    | Descripition | Step by step guide | 
| ------------- | ------------- |------------- |
| <a href="https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=BCAccelerator&amp;templateURL=https://s3.amazonaws.com/ecs-cfn-templates-101/oneclickdeployment.json" target="_blank"><span class="inlinemediaobject"><img alt="Launch Stack" src="https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/images/cloudformation-launch-stack-button.png"></a>  | Deploy smart contact accelerator without SSH access to EC2 (non-technical audience)  | <a href="https://s3.amazonaws.com/ecs-cfn-templates-101/Smartcontract-Accelerator+deployment+guide.pdf" target="_blank"> Click here</a> |
| <a href="https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=BCAccelerator&amp;templateURL=https://s3.amazonaws.com/ecs-cfn-templates-101/oneclickdeployment-ssh.json" target="_blank"><span class="inlinemediaobject"><img alt="Launch Stack" src="https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/images/cloudformation-launch-stack-button.png"></a>  | Deploy smart contact accelerator with SSH access to EC2 (for non-technical audience) | <a href="https://s3.amazonaws.com/ecs-cfn-templates-101/Smartcontract-Accelerator+deployment+guide.pdf" target="_blank"> Click here</a> |



## What is setup behind the scenes for you?

Note that a default VPC and Subnet will be established for you. The Blockchain and the Admin App run in the EC2 instance set up for you.

<img src="https://github.com/objectfrontiergit/smart-contract-accelerator/blob/master/aws/images/AWS.svg" width="750" height="450" />

## Pricing

The accelerator is free of cost. 

You will be billed only for the EC2 Instance and It depends on the EC2 instance size and how long you are running the application. Template provides an opporunity for the users to select the EC2 instance size, by default we have selected t2.small which costs ~$0.0232 per hour.  
Please refer to the link for pricing - https://aws.amazon.com/ec2/instance-types/t2/.

## FAQ's . 
  
- What AWS services are used in the application?  
Cloudformation, EC2 and Security group. It uses the default VPC to create the EC2 Instance . 
  
- How much it will cost me on AWS to run this application?  
You will be billed only for the EC2 Instance and It depends on the EC2 instance size and how long you are running the application. Template provides an opporunity for the users to select the EC2 instance size, by default we have selected t2.small which costs ~$0.0232 per hour.  
Please refer to the link for pricing - https://aws.amazon.com/ec2/instance-types/t2/ . 
  
- How can I delete the application?  
Yes, application can be deleted either by deleting the stack in the cloudformation stack or by terminating the EC2 instance. Preferred approach is to delete from the cloudformation, as it will delete even the security group.  
Steps to delete the cloudformation stack - https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-console-delete-stack.html . 

## Licence . 

See [LICENSE](LICENSE) 






