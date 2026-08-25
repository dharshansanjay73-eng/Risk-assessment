# Risk-assessment
# EXPERIMENT 4
# ASSET-ORIENTED RISK ASSESSMENT OF STORAGE ASSETS IN AWS AND AZURE
# Objective
To identify storage assets in AWS S3 and Microsoft Azure Blob Storage, identify possible vulnerabilities and threats, and assess their likelihood, impact, and risk level.

1. Software / Cloud Services Required
AWS Account 
Microsoft Azure Account 
Web Browser 
Internet Connection
Cloud Services Used
Cloud Platform	Storage Service
AWS	Amazon S3
Microsoft Azure	Azure Blob Storage
# PART A — AWS S3 STORAGE ASSESSMENT
Step 1: Login to AWS

1.Open the AWS Management Console.

2.Sign in using your AWS account. 

3.Search for S3. 


4.Select Amazon S3. 



Step 2: Select the S3 Bucket
1.Click Buckets. 

2.Select the S3 bucket created in the previous experiment
. 
3.Record: 

oBucket name 

oAWS Region 

oNumber/type of objects 


<img width="1917" height="917" alt="Screenshot 2026-08-25 134952" src="https://github.com/user-attachments/assets/f6d022f0-ca5a-42cf-a585-68f2d7e3dac6" />

Step 3: Check Block Public Access

1.Open the S3 bucket. 

2.Select Permissions. 

3.Locate Block public access (bucket settings). 

4.Check Block all public access. 

Record:

ON → Secure configuration 

OFF → Potential public-access risk 

<img width="1917" height="928" alt="Screenshot 2026-08-25 135141" src="https://github.com/user-attachments/assets/cfb6e826-a2f9-4bd0-a08b-04f2dde12893" />


Step 4: Check Bucket Versioning

1.Select the Properties tab. 

2.Locate Bucket Versioning. 

3.Record whether it is: 

oEnabled 

oDisabled 

Security purpose

Versioning helps recover previous versions of objects after accidental deletion or modification.

<img width="1527" height="277" alt="Screenshot 2026-08-25 135220" src="https://github.com/user-attachments/assets/a9753a36-dfa5-47f2-ad0b-62ccc68e2751" />


Step 5: Check Default Encryption

1.Stay in the Properties tab. 

2.Locate Default encryption. 

3.Record the encryption type.

Possible configurations include:

SSE-S3 

SSE-KMS 

DSSE-KMS

Security purpose

Encryption protects stored data from unauthorized disclosure.


<img width="1532" height="305" alt="image" src="https://github.com/user-attachments/assets/9a17c365-c1b9-4c47-b60a-242a01b455c7" />



Step 6: Check Bucket Policy

1.Select Permissions. 

2.Locate Bucket policy. 

3.Check whether a bucket policy exists. 

Record:

Policy exists 

No policy 

Note

A missing bucket policy is not automatically a vulnerability. Access may be controlled through IAM and other AWS security mechanisms.

<img width="1528" height="752" alt="Screenshot 2026-08-25 135313" src="https://github.com/user-attachments/assets/2ae95415-3c6f-492d-bb90-6d2389cdb7bb" />


Step 7: Check Object Ownership and ACL

1.In Permissions, locate Object Ownership. 

2.Record the current configuration. 

A common secure configuration is:

Bucket owner enforced

This means:

ACLs are disabled. 

Objects are owned by the bucket owner. 

Access is controlled using policies. 

<img width="1522" height="182" alt="Screenshot 2026-08-25 135354" src="https://github.com/user-attachments/assets/b35743fa-ab27-4a16-88e2-1c7e03265482" />


Step 8: Check Server Access Logging

1.Go to Properties. 

2.Locate Server access logging. 

3.Record whether it is: 

oEnabled 

oDisabled 

Security purpose

Logging helps investigate suspicious or unauthorized access to the bucket.

<img width="1532" height="160" alt="image" src="https://github.com/user-attachments/assets/6e4a5b6b-0d2b-47cb-a957-ba05cfa2c793" />

# RESULT:
The storage assets in AWS S3 were identified and analyzed. Various security configurations, vulnerabilities, threats, likelihood, and impacts were evaluated. Risk scores were calculated using the Likelihood × Impact method, and appropriate security mitigation measures were recommended.
