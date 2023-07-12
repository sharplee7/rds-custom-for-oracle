# rds-custom-for-oracle

### You'll need to generate a symmetric-key encryption key using the Amazon Key Management System (KMS) beforehand.
#### 1. goto your aws cloudformation console, upload codebuild-vpc-infra.yaml and run script
#### 2. upload codebuild-vpc-endpoints.yaml and run it on CloudFormation
#### 3. uplolad custome-oracle-iam.jason and run it on CloudFormation
#### 4. Prepare your own Oracle installation files
#### 5. Create an S3 bucket and upload the prepared Oracle Installation file to it (in the form of a zip file)
#### 6. In the AWS Web Console, find the 'Custom engine versions' menu for RDS, click the 'Create custom engine version' button and create an RDS creation image from the Oracle Installation image you uploaded to S3.
#### 7. Finally, create the RDS Oracle. Make sure to create the RDS from the "Custom Engine Version" you created earlier. For VPCs and subnets, select the VPC and subnet you created in CloudFormation earlier.

#### You are now finished.