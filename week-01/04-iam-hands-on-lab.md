# Day 4 - IAM Hands-On Lab

Goal: Practice least privilege using IAM users, groups, and policies.

## Lab 1 - S3 Read-Only Access

Create:

- Group: `S3ReadOnlyGroup`
- Policy: `AmazonS3ReadOnlyAccess`
- User: `learner-s3`

Test:

- Confirm the user can view S3.
- Try one action that should fail.
- Capture the `Access Denied` result.

## Lab 2 - EC2 Read-Only Access

Create:

- Group: `EC2ReadOnlyGroup`
- Policy: `AmazonEC2ReadOnlyAccess`
- User: `learner-ec2`

Test:

- Confirm the user can open the EC2 dashboard.
- Confirm the user cannot create or terminate instances.

## Lab 3 - Billing Read-Only Access

Create:

- Group: `BillingViewGroup`
- Policy: `AWSBillingReadOnlyAccess`
- User: `learner-billing`

Test:

- Confirm the user can view the Billing Dashboard.
- Confirm the user cannot manage unrelated AWS services.

## Lab 4 - Custom S3 Read-Only Policy

Create a customer managed policy:

```text
CustomS3ReadOnlyTrainingPolicy
```

Use this structure and replace `YOUR-BUCKET-NAME`:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    { "Effect": "Allow", "Action": ["s3:ListAllMyBuckets"], "Resource": "*" },
    { "Effect": "Allow", "Action": ["s3:ListBucket"], "Resource": "arn:aws:s3:::YOUR-BUCKET-NAME" },
    { "Effect": "Allow", "Action": ["s3:GetObject"], "Resource": "arn:aws:s3:::YOUR-BUCKET-NAME/*" }
  ]
}
```

Deliverables:

- Screenshots of group, user, and attached policy.
- Screenshot of allowed access.
- Screenshot or note for denied access.
- Policy JSON file in your submission folder.
