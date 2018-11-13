# Deploy OFS SmartContract Accelarator in AWS with one click







![aws deployment](https://github.com/objectfrontiergit/smart-contract-accelerator/blob/master/aws/images/AWS.svg)  






| Buttons    | Descripition | Playbook link | 
| ------------- | ------------- |------------- |
| <a href="https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=BCBOneClickDeployment&amp;templateURL=https://github.com/objectfrontiergit/smart-contract-accelerator/blob/master/aws/oneclickdeployment.json" target="_blank"><span class="inlinemediaobject"><img alt="Launch Stack" src="https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/images/cloudformation-launch-stack-button.png"></a>  | Deploy smart contact accelerator without SSH access to EC2  | Click here |
| <a href="https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=BCBOneClickDeployment&amp;templateURL=https://github.com/objectfrontiergit/smart-contract-accelerator/blob/master/aws/oneclickdeployment-ssh.json" target="_blank"><span class="inlinemediaobject"><img alt="Launch Stack" src="https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/images/cloudformation-launch-stack-button.png"></a>  | Deploy smart contact accelerator with SSH access to EC2  | Click here |







# FAQ's . 
- Do I need to have AWS account?  
Yes, you need to have an active AWS account to run the smartcontract accelerator application.  
  
- How to create a new AWS account?  
Please follow the steps listed in the link https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/  
  
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


