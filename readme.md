![ga4](https://www.google-analytics.com/collect?v=2&cid=1&sid=1&tid=G-564TXM315H&en=page_view&dl=workloadidentityfederation&dt=readme.md)

# Workload Identity Federation

Workload identity federation (WIF) is a way to authenticate workloads in Google Cloud without the need of service account keys. 

This works by establishing a trust relationship between an external identity provider (IdP), such as GitHub, AWS, Azure, and Google Cloud. Once that trust relationship is created, your software workload can exchange trusted tokens from the external IdP for access tokens from Google Cloud. Your software workload then uses that access token to access the protected resources to which the workload has been granted access. This eliminates the maintenance burden of manually managing credentials and eliminates the risk of leaking secrets or having certificates expire.

# Why Use Workload Identity Federation?
This can be beneficial for a number of reasons, including:

* Security: Service account keys are powerful credentials that can present a security risk if they are not managed correctly. Workload identity federation eliminates the need to manage service account keys, reducing the risk of unauthorized access.
* Convenience: Workload identity federation can make it easier to manage access to cloud resources. With workload identity federation, you can use Identity and Access Management (IAM) to grant external identities IAM roles, including the ability to impersonate service accounts. This approach eliminates the maintenance and security burden associated with service account keys.
* Compliance: Workload identity federation can help you comply with security and compliance requirements. For example, the Payment Card Industry Data Security Standard (PCI DSS) requires that service account keys be encrypted when stored. Workload identity federation eliminates the need to store service account keys, which can help you comply with PCI DSS requirements.

## Google Disclaimer
This is not an officially supported Google product

## Example Repositories
| Provider |  Description | Example Code  |
| :---- | :----   | :--- |
| AWS | This code demonstrates an AWS Lambda Function calling the Google Cloud Vision API using the Google Cloud SDK via Workload Identity Federation. | https://github.com/dreardon/gcp-workload-identity-federation-aws-lambda-sdk |
| AWS | This code demonstrates an AWS EC2 Instance calling the Google Cloud Vision API using the Google Cloud SDK via Workload Identity Federation. | https://github.com/dreardon/gcp-workload-identity-federation-aws-ec2-sdk |
| AWS | This code demonstrates an AWS Lambda function calling the Google Cloud Vision API using REST via Workload Identity Federation. | https://github.com/dreardon/gcp-workload-identity-federation-aws-lambda-rest |
| AWS | This code demonstrates an AWS EC2 Instance calling the Google Cloud Vision API using REST via Workload Identity Federation. | https://github.com/dreardon/gcp-workload-identity-federation-aws-ec2-rest |
| Okta | This code demonstrates an Okta custom application to exchange credentials for short-lived Google Cloud credentials via Workload Identity Federation.  | https://github.com/dreardon/workload-identity-okta |
