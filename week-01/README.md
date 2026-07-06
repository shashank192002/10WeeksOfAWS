# Week 1 - Cloud Foundations + IAM

AWS Zero To Hero - CloudAdhar x TrainWithShubham  
Sessions: Jul 4-5, 2026  
Exam focus: SAA-C03 Domain 1 - Design Secure Architectures  
Main pillar: Security

Week 1 is about building a safe AWS foundation before touching EC2, S3, VPC,
databases, or production-style architecture.

## Weekly Outcome

By the end of this week, you should be able to:

- Explain Regions, Availability Zones, and Edge Locations.
- Explain the AWS Shared Responsibility Model.
- Secure the AWS root user with MFA.
- Create billing or budget alerts.
- Explain IAM users, groups, roles, and policies.
- Apply least privilege using read-only access.
- Read a basic IAM JSON policy.
- Understand why temporary credentials are safer than long-lived access keys.

## 5-Day Practice Sequence

| Seq | When | Practice | File |
|---:|---|---|---|
| 01 | Day 1 | Learn cloud foundations | [01-cloud-foundations.md](./01-cloud-foundations.md) |
| 02 | Day 2 | Learn IAM basics | [02-iam-basics.md](./02-iam-basics.md) |
| 03 | Day 3 | Secure AWS account and billing | [03-account-security-lab.md](./03-account-security-lab.md) |
| 04 | Day 4 | Practice IAM users, groups, and policies | [04-iam-hands-on-lab.md](./04-iam-hands-on-lab.md) |
| 05 | Day 5 | Try optional GitHub OIDC challenge | [05-github-oidc-challenge.md](./05-github-oidc-challenge.md) |
| 06 | End of week | Clean up test AWS resources | [06-cleanup.md](./06-cleanup.md) |
| 07 | End of week | Submit your weekly work | [07-submission-format.md](./07-submission-format.md) |
| 08 | End of week | Post learning update on LinkedIn | [08-linkedin-post.md](./08-linkedin-post.md) |
| 09 | Before next week | Revise for quiz | [09-quiz-prep.md](./09-quiz-prep.md) |

## Submission

- Use this structure: [07-submission-format.md](./07-submission-format.md)
- Clean up test resources: [06-cleanup.md](./06-cleanup.md)
- Post daily progress: [08-linkedin-post.md](./08-linkedin-post.md)
- Prepare for next week quiz: [09-quiz-prep.md](./09-quiz-prep.md)

## Exam + Pillar Mapping

| Topic | Exam Mapping | Pillar | Best Practice |
|---|---|---|---|
| Root MFA | Domain 1 | Security | Protect root user |
| Billing alerts | Domain 4 | Cost Optimization | Monitor cost early |
| Shared responsibility | Domain 1 | Security | Know AWS vs customer duties |
| IAM groups | Domain 1 | Security | Manage permissions centrally |
| IAM roles | Domain 1 | Security | Prefer temporary access |
| IAM policies | Domain 1 | Security | Use least privilege |
| GitHub OIDC | Domain 1 | Security | Avoid long-lived access keys |

## Rules

- Do not share access keys, secret keys, MFA QR codes, payment details, or
  sensitive billing screenshots.
- Use your own AWS account carefully.
- Prefer Free Tier resources and delete test resources after labs.
- Share progress publicly, but hide sensitive information.

<div align="center">

[Home](../README.md) | [Week 2](../week-02/)

</div>
