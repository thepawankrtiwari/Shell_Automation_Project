# Shell_Automation_Project

## Script to automate the process of listing all the resources in an AWS account
#
### Below are the services that are supported by this script:
1. EC2
2. RDS
3. S3
4. CloudFront
5. VPC
6. IAM
7. Route53
8. CloudWatch
9. CloudFormation
10. Lambda
11. SNS
12. SQS
13. DynamoDB
14. VPC
15. EBS
#
### The script will prompt the user to enter the AWS region and the service for which the resources need to be listed.
#
- Usage: ./aws_resource_list.sh  <aws_region> <aws_service>
- Example: ./aws_resource_list.sh ap-southeast-2 ec2


### Here you can understand more clearly in simple words, I'm trying in different words:

Example Scenario:
Imagine a company that rents several virtual "rooms" in a cloud data center. 
Each "room" (like EC2 instances, S3 buckets, etc.) costs money based on its usage, 
similar to renting space in a building. 
The company wants to ensure it's not paying for any unused or unnecessary "rooms."

### Script Actions Step-by-Step:

- The script begins by checking all the "rooms" (cloud resources) the company is renting in a specific region of the cloud (like us-east-1 or us-west-2).
  
  **Example in Simple Terms**: Think of this as a caretaker starting their round to check which rooms in a large hotel are currently occupied or in use.
Lists All Active "Rooms" (Resources)

- It creates a list of all the active "rooms" (such as virtual servers, storage spaces, and databases) that are currently being used in that region.
  The script identifies any "rooms" that are not actively being used but are still being paid for, such as idle servers or empty storage spaces.
  
  **Example in Simple Terms**: The caretaker writes down the room numbers and details of all the rooms that have guests or are being used for storage.
   Checks for Unused or Unnecessary "Rooms"
  The caretaker checks if there are any rooms that are empty but still have the lights on, with no one inside.
   Prepares a Report of Findings

- After listing all active resources and identifying unused ones, the script compiles this information into a report.

    **Example in Simple Terms**: The caretaker writes a summary report listing all the occupied rooms and highlighting which rooms are empty but still have the lights on.
    Sends the Report to the Operations Team

- The script automatically sends this report via email to the operations department of the company.

    **Example in Simple Terms**: The caretaker sends a copy of the report to the hotel manager, so they know which rooms are in use and which ones are wasting electricity.
      Enables Cost Optimization

- The operations team can then decide which unused "rooms" (cloud resources) to turn off or stop paying for, saving money.
  
    **Example in Simple Terms**: The hotel manager decides to turn off the lights in the empty rooms and possibly stop renting those rooms, reducing the electricity bill and saving money.

