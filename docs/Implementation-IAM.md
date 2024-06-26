## Identity Access Management

Following the model of least privilege is always the best practice. We do not want to give away the keys to the kingdom which is why we must segregate our workloads and resources. As you can see in this diagram below we want to be able to assume roles from our management account into our other OUs(Organizational Units)

![image](https://github.com/Algoroy27/GRC/assets/137920855/c261d591-8add-4166-b870-497962624948)



## Step 1 Create IAM Roles in the Target Accounts

Log in to each target account (Production, Development, Test) and create an IAM role that the management account can assume.

Go to the IAM console.
- Click on "Roles" and then "Create role".
- Select "Another AWS account" as the trusted entity.
- Enter the account ID of the management account.
- Attach the necessary policies that grant the permissions you want the role to have in the target account.
- Complete the role creation process and take note of the Role ARN


## Step 2: Create IAM Policies in the Management Account
- Log in to your management account and create a policy that allows assuming the roles created in the target accounts.

- Go to the IAM console.

- Click on "Policies" and then "Create policy".

- Add the following JSON to allow assuming roles:

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "sts:AssumeRole",
      "Resource": [
        "arn:aws:iam::ACCOUNT_ID_PRODUCTION:role/ROLE_NAME",
        "arn:aws:iam::ACCOUNT_ID_DEVELOPMENT:role/ROLE_NAME",
        "arn:aws:iam::ACCOUNT_ID_TEST:role/ROLE_NAME"
      ]
    }
  ]
}
