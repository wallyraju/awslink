Team Echelon: 

Members:

Philippe Kabore - AWS Administrator

Lavasha Holden - Scribe

Developers: 
Philippe Kabore
Zachary Sinclair
Matthew Herman
Felix Arroyo
Lavasha Holden
Wally Bhupatiraju
=====================================

Application: Recipe Application

Our Application is a Website that is hosted in AWS that is used for storing and displaying user created Recipes. The following capabilities are available in our application
There are four pages to the website, 
    Home Page
    Recipes Page
    Login
    Registration

=====================================

Application Features: 

1. Register for a user account. An existing email address and a password with some minimum requirements is needed to register for an account. 
    When you register, you will receive a code to your email that you will need to verify your account. 
    Once you verify your account, you will be allowed to log in and then submit a recipe to the website.
2. You will be able to Login once you have a registered user account and then can submit a recipe.
3. View already submitted recipes.
4. Visit the Home page of the web site. 

=====================================

Architecture

Our application's architecture consists of the following components

1. GitHub - For hosting the source code repository. Our repository has a master branch.
2. AWS Amplify - We used AWS Amplify to develop the front end of our application. Amplify was setup to connect to our Github repository. When any check-in is made to the master branch repository, these changes are automatically applied in AWS Amplify.
3. Dynamo DB - We used Dynamo DB as the back end Database for the application for storing and retrieving recipes.
4. Cognito - This is used for User management, authentication and verification.
5. API Gateway - A fully managed service that allows developers to create, publish, maintain, monitor, and secure APIs. We have used it to save to and retrieve recipes from the database.
6. Lambda Functions - Used for running code without provisioning servers. Used in conjunction with API Gateway to support the application.
7. AWS Cloudwatch - Used for monitoring the application in real time. We used it to create a log group for the Lambda function.

=======================================

Demo:

For today's demo we will show 

1. A user registering to the website and verifying their account
2. The same user logging in to the application
3. The user adding a recipe
4. The user viewing existing recipes on the web site.

=======================================

Cost:

So far we have noticed that the cost for running the application for the purpose of the demo has cost us next to nothing

=======================================

Lessons Learned/Still learning

1. We are able to copy the entire application from a team member's AWS account to the AWS account provided for the purpose of this class in under 60 minutes and have it up and running. 
2. We ran into some issues with retrieing the data from the database back to the application front end, so for the purpose of the demo, we have used a static web page with a select few recipes.

========================================
