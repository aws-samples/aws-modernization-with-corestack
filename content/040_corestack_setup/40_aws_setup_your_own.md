---
title: "1. CoreStack Account Setup"
chapter: true
weight: 10
---

## CoreStack Account Setup

Please go to the [CoreStack Dashboard](https://cloud.corestack.io/). Login with the email and password you used to sign up! There should be a confirmation email sent with your login information. Your greeting page should look like this:
![CoreStack Dashboard](/images/corestack-dashboard.png)

1. Click the **GET STARTED** button and choose AWS as the public cloud on the next page
   ![Cloud to Start](/images/corestack-start.png)
1. Click the Assessment + Governance option, Linked Account option, AWS Standard option, and the AssumeRole authentication option. Click the **NEXT** button.
   ![CoreStack Configuration](/images/corestack-configuration.png)
1. Next, go to your AWS Management Console and search for the CloudFormation dashboard.
1. Click the create stack option and copy this link [CoreStack Role Creation Template](https://corestack-cfn.s3.amazonaws.com/AWS_Create_IAM_Role_For_CorestackAssessmentandGovernance_content.json) and paste it into the Amazon S3 URL
   ![Role Creation](/images/cfn-role-create-stack.png)
1. Name the stack ``CoreStack-Role-Stack``, the externalId as some value, and RoleName as ``CoreStackAccessRole``.
1. Click through and create the stack.
1. Once the stack has finished provisioning, click on the stack and click on the outputs tab:
   ![CoreStack-Role-Stack Output](/images/cloudformation-output-tab.png)
1. There should be 3 outputs: the externalID you submitted, whether MFA is enabled (it should be set to false), and the role ARN. Copy the ARN and ExternalID
1. Go back to your CoreStack dashboard and paste the 2 values you copied from the step before and click the **VALIDATE** button.
1. Drop down and select the region you used to create the CloudFormation stack for the role. Click the **I'M DONE** button, and you have now successfully linked your AWS account to CoreStack!!

Let's moe the next section 