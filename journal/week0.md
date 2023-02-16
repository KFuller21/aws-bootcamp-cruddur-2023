# Week 0 — Billing and Architecture

Recreate Logical Architectual Diagram in Lucid Charts: journal/Cruddur - Diagram.pdf | https://github.com/KFuller21/aws-bootcamp-cruddur-2023/blob/0d2dcb03fa8f8b8ebbeddb89ec8dc922298569ae/journal/Cruddur%20-%20Diagram.pdf



# Creating an AWS organization involves the following steps:

1. Sign in to your AWS account as the root user.
2. Navigate to the AWS Organizations console.
3. Choose "Create organization" and select "Consolidated billing" or "All features" depending on your needs.
4. Choose a name for your organization and enter an email address for the master account.
5. Review the information and create the organization.
6. Once the organization is created, you can create accounts and move existing accounts into the organization.
7. You can then assign policies to the accounts to manage their access to resources and services.

By creating an AWS organization, you can centralize billing and management of multiple AWS accounts and apply policies to them.


# To generate IAM credentials and log into AWS CLI, follow these steps:

1. Log in to the AWS Management Console as an IAM user with appropriate permissions.
2. Navigate to the IAM console and select the user for whom you want to generate the credentials.
3. In the "Security credentials" tab, choose "Create access key".
4. Download the generated access key and secret key.
5. Install and configure the AWS CLI on your local machine.
6. Open a command prompt and enter the "aws configure" command.
7. Enter the access key, secret key, default region, and output format when prompted.
8. Once you have configured the AWS CLI, you can log in by entering the "aws configure" command followed by the desired AWS service and command.
For example, to list all EC2 instances in your account, you can enter "aws ec2 describe-instances".

By generating IAM credentials and logging into AWS CLI, you can access and manage AWS resources using a command-line interface.

# To create an AWS billing alarm, follow these steps:

1. Sign in to the AWS Management Console and navigate to the CloudWatch console.
2. In the navigation pane, choose "Alarms" and then choose "Create alarm".
3. Choose "Select metric".
4. Under "Metric namespaces", choose "AWS/Billing".
5. Under "Select metric", choose "Total Estimated Charge".
6. Select the appropriate time range for which you want to monitor your charges.
7. Choose the "Create new alarm" button.
8. Configure the conditions for the alarm, such as the threshold amount and the actions to be taken when the threshold is exceeded.
9. Choose "Create alarm".

Once the billing alarm is created, you will receive notifications when your estimated charges reach the threshold you set. You can also view your billing data and create reports in the Billing and Cost Management console.

# To create an AWS zero spend budget, follow these steps:

1. Sign in to the AWS Management Console and navigate to the Billing and Cost Management console.
2. In the navigation pane, choose "Budgets" and then choose "Create a budget".
3. Choose "Cost budget" and select the appropriate budget type.
4. Enter a name and description for the budget.
5. Choose the appropriate time period for the budget.
6. Choose "Use a custom cost filter".
7. Under "Filter", select "Service" and choose "All services".
8. Under "Filter", select "Usage type" and choose "All usage types".
9. Under "Filter", select "Operation" and choose "All operations".
10. Under "Filter", select "Tag" and choose "Any tag".
11. In the "Amount" field, enter "0".
12. Configure the other budget options as desired and choose "Create budget".

Once the budget is created, you will receive alerts when any costs are incurred that exceed the budgeted amount of zero. You can view your budget and its details in the Budgets dashboard in the Billing and Cost Management console.

# Final Thoughts:
While preparing for the bootcamp, I already had registered a domain in an AWS Account I used for the popular Cloud Resume Challenge. I am hoping to use this domain with this project and just add on to the 'Portfolio' area of by site. I created two accounts, one for Production and one for Development so I can practice using different deployment environments. I am excited for week two!

