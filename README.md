# AWS-Cognito-Service


 Amazon	Cognito	
 
AWS Cognito User Pool Service.
Glossary


AWS Cognito - Service that provides authentication, authorization, and user

management for web and mobile apps. Users can sign-in directly with a

username and password or through a third party such as Azure AD, Amazon, or

Google. Amazon Cognito consists of two main components: user pools and

identity pools. User pools are user directories that provide sign-up and sign-in

options for app users. Identity pools enable you to grant your users access to

other AWS services. You can use identity pools and user pools separately or

together.


AWS Cognito consists two services 1. User pools
2. Identity Pools


User pools-

A user pool is a user directory in Amazon Cognito. With a user pool, your users can sign

in to your web or mobile app through Amazon Cognito. Your users can also sign in

through social identity providers like Google, Facebook, Amazon, or Apple, and through

SAML identity providers.

User Pools Providing:-



• Sign-up and sign-in services.

• A built-in, customizable web UI to sign in users.

• Social sign-in with Facebook, Google, Login with Amazon, and Sign in with Apple,

as well as sign-in with SAML identity providers from your user pool.

• User directory management and user profiles.

• Security features such as multi-factor authentication (MFA), checks for

compromised credentials, account takeover protection, and phone and email

verification.

• Customized workflows and user migration through AWS Lambda triggers.


Identity Pools:-
Amazon Cognito identity pools (federated identities) enable you to create unique

identities for your users and federate them with identity providers. With an identity

pool, you can obtain temporary, limited-privilege AWS credentials to access other

AWS services.


Creating User Pools
Click on Manger User pools
After click on Manger User pools then you can create User pools
Click On Create User Pools

Pool Name-Enter Pool Name
Example:TestPool


There are two ways to create user pool • Review default -
• Which we can review the by start and customize setting as desired • Step Through settings-
• We can through each step and customize the settings

Click on Attribute
Which we can customize end user sign in

The End user can sign two ways either by Username and Email address or phone Number


Leave all settings default (if you don’t want to set some)
Go to review page and review it and create the pool



Click on Create Pool

Click on App Client
So, App Client will give the Unique ID and Optional secret key to access User Pool


Enter App Client Name
Then to create App client Name click on Create app client


Then, will get App client ID and App Client Secret

Go to App Client Setting in App Integration
In App Client Setting, We have to enable at least one identity provider for each app client either identity providers or OAuth 2.0 settings


Enabled Identity Providers

Checked Cognito User pool Enter call back URLs

OAuth 2.0
Checked the Authorization code for back-end authorization and implicit grant will give the JWT Tokens and select all Allowed OAuth Scopes.


Go to Domain Name Enter The Domain Name

Go to App Integration for Domain Name and open the URL

https://test006.auth.us-east-2.amazoncognito.com/login?response_type=token&client_id=2sfbhnskh6tal6hjj1n9rbd4j7&redirect_uri=https://www.example.com


You need to add some parameter like
• App Client ID which is in App Clients
• redirect_uri which is in app client Settings(Callback URL)

Then we can see the AWS Cognito Sign in page

To access the website, we need to sign up by entering following
• User Name • E-mail
• Password
Then we will get the verification code to entered E-mail Address

Once verification is done, then user will be enabled and access the domain
