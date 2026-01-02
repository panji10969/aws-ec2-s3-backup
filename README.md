# aws-ec2-s3-backup
belajar membuat project aws


## Project Overview

Project ini adalah demo AWS cloud solution ke automate EC2 backup files ke amazon S3 menggunakan AWS Free Tier Services.
Tujuan project ini untuk simulasi dunia nyata pekerjaan cloud operation, dimana EC2 instance generate backup files dan upload secara aman ke S3 bucket menggunakan IAM best practices.

## Solution Architecture

EC2 instance adalah konfigurasi untuk generate backup files dan upload ke amazon S3 bucket menggunakan AWS CLI.
IAM Roles dan access policie ensure secure access.
S3 versioning dan lifecycle policies di aktikfkan untuk improve data protection dan cost efficiency.

EC2 Instance
    |
    | AWS CLI (IAM Role)
    v
S3 Bucket (Versioning + Lifecycle)


## AWS Services Used

- Amazon EC2 (Free Tier) – compute instance
- AWS IAM – access management and security
- Amazon S3 – object storage for backups
- Amazon CloudWatch – basic monitoring
- AWS CLI – automation tool

## Implementation Steps

1. Created an IAM user with limited S3 access
2. Launched an EC2 instance using Amazon Linux
3. Installed AWS CLI on EC2
4. Generated a sample backup file
5. Uploaded the backup file to Amazon S3
6. Enabled S3 Versioning
7. Configured Lifecycle policy for cost optimization

## Security & Cost Consideration

- IAM permissions follow the principle of least privilege
- S3 bucket access is private
- No public access is allowed
- Lifecycle rules are used to reduce storage cost
- All resources stay within AWS Free Tier limits

## Result & Learning

Project ini berhasil mendemonstrasikan dasar alur kerja cloud backup.
Dengan project ini, saya bisa merasakan pengalaman dengan AWS IAM, EC2, S3 dan cloud security best practice.
Ini juga improved pengetahuan saya tentang cost optimization di cloud environments.
