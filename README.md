# AWS Cloud Security Lab

A hands-on cloud security project demonstrating 
real-world AWS infrastructure setup, IAM 
least-privilege design, and secure CI/CD 
pipeline implementation.

---

## What This Project Covers

### IAM Least-Privilege Architecture
- Separated admin and daily-driver IAM identities
- Created scoped policies for EC2, S3, and CloudTrail
- Enforced MFA on all identities
- Eliminated AdministratorAccess from daily-use accounts

### S3 Security Controls
- Configured Block Public Access settings
- Built and debugged bucket policies
- Simulated a public exposure scenario
- Performed full remediation and verified closure

### EC2 Security & Network Auditing
- Launched and secured an EC2 instance
- Connected via SSH using key pair authentication
- Audited open ports using netstat
- Analyzed Security Group inbound/outbound rules
- Identified egress filtering gap as residual risk

### CloudTrail Audit Logging
- Investigated security-relevant API events
- Reconstructed incident timeline from event history
- Tracked PutBucketPolicy and 
  PutBucketPublicAccessBlock events

### Secretless CI/CD Pipeline
- Built GitHub Actions workflow deploying to AWS S3
- Implemented OIDC trust relationship 
  (no stored credentials)
- Debugged multi-layer trust policy mismatches
- Scoped role trust to specific repo and branch

---

## Technologies Used
- AWS (EC2, S3, IAM, CloudTrail, GuardDuty, VPC)
- GitHub Actions
- OIDC Authentication
- Linux / Terminal
- Git

## Certifications
- AWS Certified Cloud Practitioner
- Google Cybersecurity Certificate
- AWS Solutions Architect Associate (SAA-C03) 
  — In Progress
