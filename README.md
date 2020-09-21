# Amazon Comprehend for Natural Language Processing (NLP)

## Using Amazon Comprehend through AWS Console
### Preparation steps for using Comprehend through the console
1. Create account at Amazon AWS
2. Create an S3 bucket for your files

### Amazon Comrehend analysis through Console
1. Prepare your data. I used Twitter API to clreate a .csv files for specific queries. 
2. Upload your data into your S3 bucket. Create a separate folder for the resutls.
3. Create Analysis Job for your analysis.
4. Once the job finishes running, download the output file.
5. Process the JSON output to understand the results.
https://github.com/tanyazyabkina/AmazonComprehend/blob/master/AWS_Comprehend_JSON_to_CSV.ipynb

## Using Amazon Comprehend through the API
### Preparation steps for using Comprehend through the API
1. Create account at Amazon AWS
2. Create an admin user in IAM and get the access keys
3. Install AWS Command Line Interface (AWS CLI) and configued itto use your access keys
4. Create an S3 bucket for your file
5. Install python packages: boto3, pandas, json
### Analyze text using Amazon Comprehend API
1. Upload your data into S3 bucket.
2. Create analysis job.
3. Run analysis job.
4. Download results from S3 bucket.
5. Process the JSON output to understand the results.
https://github.com/tanyazyabkina/AmazonComprehend/blob/master/AWS_Comprehend_JSON_to_CSV.ipynb
