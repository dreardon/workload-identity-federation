# Workload Identity Federation

Workload identity federation (WIF) is a way to authenticate workloads in Google Cloud without the need of service account keys. 

This works by establishing a trust relationship between an external identity provider (IdP), such as GitHub, AWS, Azure, and Google Cloud. Once that trust relationship is created, your software workload can exchange trusted tokens from the external IdP for access tokens from Google Cloud. Your software workload then uses that access token to access the protected resources to which the workload has been granted access. This eliminates the maintenance burden of manually managing credentials and eliminates the risk of leaking secrets or having certificates expire.

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