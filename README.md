# Cloud Security - Programmability

##### Security Center Terraform Module
https://github.com/kumarvna/terraform-azurerm-security-center

##### Getting into Azure With Terraform
https://dev.to/jevason90/getting-into-azure-with-terraform-264b

##### Securely Deploy Azure Infrastructure w/ Terraform
https://blog.azureandbeyond.com/2019/01/24/how-to-securely-deploy-azure-infrastructures/

##### Azure Active Directory Security Group Automation With Power Automate
https://medium.com/marcus-tee-anytime/azure-active-directory-security-group-automation-with-power-automate-1aee7bab28c3

##### Understanding API connections for your Azure Sentinel Playbooks
https://techcommunity.microsoft.com/t5/azure-sentinel/understanding-api-connections-for-your-azure-sentinel-playbooks/ba-p/2593973

##### End to End Cloud Security Automation With Terraform
https://www.youtube.com/watch?v=WXhOW0gvlTU

##### Getting Into Azure With Terraform
https://dev.to/jevason90/getting-into-azure-with-terraform-264b

##### Azure Policies With Terraform
https://www.youtube.com/watch?v=P5HElJxJdbk

##### Palo Alto Terraform Templates
https://github.com/PaloAltoNetworks/terraform-templates

##### Palo Alto Terraform Templates
https://github.com/PaloAltoNetworks/terraform-templates

##### Pan-OS Python
https://github.com/PaloAltoNetworks/pan-os-python

##### Palo Alto Cloud Integration
https://live.paloaltonetworks.com/t5/cloud-integration/ct-p/Cloud_Templates

# Cloud Security - AWS CLI
AWS CLI Command | Syntax 
------------ | -------------
S3 Bucket Creation | ```aws s3 mb s3://bucketname-01```
S3 Delete Bucket | ```aws s3 rb s3://bucketname-01 --force```
S3 List Buckets | ```aws s3 ls```
S3 List Bucket Files | ```aws s3 ls s3://bucketname-01```



# CloudTrail Logging & Auditing
##### list all trails
aws cloudtrail describe-trails

##### list all S3 buckets
aws s3 ls

##### create a new trail
aws cloudtrail create-subscription \
    --name awslog \
    --s3-new-bucket awslog2016

##### list the names of all trails
aws cloudtrail describe-trails --output text | cut -f 8

##### get the status of a trail
aws cloudtrail get-trail-status \
    --name awslog

##### delete a trail
aws cloudtrail delete-trail \
    --name awslog

##### delete the S3 bucket of a trail
aws s3 rb s3://awslog2016 --force

##### add tags to a trail, up to 10 tags
aws cloudtrail add-tags \
    --resource-id awslog \
    --tags-list "Key=log-type,Value=all"

##### list the tags of a trail
aws cloudtrail list-tags \
    --resource-id-list 

##### remove a tag from a trail
aws cloudtrail remove-tags \
    --resource-id awslog \
    --tags-list "Key=log-type,Value=all"


# Cloud Security - IAM Concepts

##### Why is IAM Important?
https://www.ibm.com/topics/identity-access-management

##### AWS SSO vs RBAC IAM Access
https://hackernoon.com/an-introduction-to-aws-sso-vs-cross-account-role-based-iam-access-60263zc1

##### Securing Your Application by Using OpenID Connect and Azure AD
https://docs.microsoft.com/en-us/learn/modules/secure-app-with-oidc-and-azure-ad/

##### Authentication vs. Federation vs. SSO
https://medium.com/@robert.broeckelmann/authentication-vs-federation-vs-sso-9586b06b1380

##### AWS IAM vs AWS SSO
https://jumpcloud.com/blog/aws-iam-vs-aws-sso

##### How It Works: Azure AD MFA
https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks

### Topology Examples:

![SAML SSO Diagram](https://user-images.githubusercontent.com/87448126/127930799-f7f85c4d-89ee-4db4-b661-a5dd623beb14.png)

![azure](https://user-images.githubusercontent.com/87448126/127947311-a0280959-4fd9-4039-ba3f-bde9804741cb.png)




# Cloud Network Infrastructure Concepts

##### Building Azure Infrastructure With Terraform
https://www.youtube.com/watch?v=d6EOEXxMZ8w



