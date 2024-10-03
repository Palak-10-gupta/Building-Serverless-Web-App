# Building-Serverless-Web-App

## Step1:Create a DynamoDB table
name:registration-table

## Step2:Create IAM role for lambda function
name:RegistrationRoleForm

##  Step3:Create lambda function
name:registration-form-function

##  Step4:Write lambda function
###### Change    (  'https://r3u6mpiyr2.execute-api.ap-south-1.amazonaws.com/prod')
###### To this: ('API_URL/register')


##  Step5:Create and deploy API Gateway and Enable CORS

##  Step6:Test the project.Registration is successful

##  Enable CORS:

###### Access-Control-Allow-Origin: '*'
###### Access-Control-Allow-Headers: Content-Type,X-Amz-Date,Authorization,X-Api-Key,X-Amz-Security-Token
###### Access-Control-Allow-Methods: POST


