# CLOUDAWS
 SIMPLE CDN TO DELIVER STATIC CONTENT IMAGE FROM CLOUD STORAGE 
STEP 1:
Create a general purpose S3 bucket in AWS and the already present settings can be kept 

STEP 2:
Upload image and a simple html file(which is provided in repo) in bucket

STEP 3:
Go to AWS Cloudfront and create a distribution , 
enter your origin's domain and name

STEP 4:
Origin access-original access settings and create new OAC, rest settings can be kept same

STEP 5:
Keep Cache policy to cacheoptimized and WAF to Do not enable security protections.
Keep all other settings same and create distribution.

STEP 6:
After creation of distribution, You must update the S3 bucket policy,
CloudFront will provide you with the policy statement after creating the distribution.(copy that code)

STEP 7:
Go back to S3 bucket, go to permissions and update bucket policy (paste the code there) then save changes.

STEP 8:
go back to cloudfront and wait for the distribution to show Enabled.

STEP 9:
 Then open distribution and copy the Distribution domain name

STEP 10:
Paste the Distribution domain name in any web server .
