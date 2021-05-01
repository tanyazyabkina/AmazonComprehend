# Amazon Comprehend for Natural Language Processing (NLP)

## Cost
If you are using free AWS tier, you can analyze 50K units a month free. A unit is 100 characters. In my example, every tweet is ~2 units. In the scheduled job I am analyzing 10K tweets at once, so the free tier limit runs out pretty fast, and then it's \$1 per 10K. Be sure to check pricing before you proceed. https://aws.amazon.com/comprehend/pricing/

## Using Amazon Comprehend through AWS Console
### Preparation steps for using Comprehend through the console
1. Create account at Amazon AWS
2. Create an S3 bucket for your files

### Amazon Comrehend analysis through Console
My blog post with screenshots: https://zyabkina.com/no-code-natural-language-processing-with-amazon-comprehend/

1. Prepare your data. I used Twitter API to clreate a .csv files for specific queries.
https://github.com/tanyazyabkina/AmazonComprehend/blob/master/get_tweets_for_terms.ipynb
2. Upload your data into your S3 bucket. Create a separate folder for the resutls.
3. Create Analysis Job for your analysis.
4. Once the job finishes running, download the output file.
5. Process the JSON output to understand the results.
https://github.com/tanyazyabkina/AmazonComprehend/blob/master/AWS_Comprehend_JSON_to_CSV.ipynb

## Using Amazon Comprehend through the API

### Preparation steps for using Comprehend through the API
1. Create account at Amazon AWS
2. Create an admin user in IAM and get the access keys
3. Install AWS Command Line Interface (AWS CLI) and configued it to use your access keys
4. Create an S3 bucket for your file
5. Install python packages: boto3, pandas, json,tarfile
### Analyze text using Amazon Comprehend API
1. Prepare your data. I used Twitter API to clreate a .csv files for specific queries.
https://github.com/tanyazyabkina/AmazonComprehend/blob/master/get_tweets_for_terms.ipynb
2. Upload your data into S3 bucket.
3. Create analysis job.
4. Run analysis job.
5. Download results from S3 bucket.
6. Process the JSON output to understand the results.

Code for 2-6: https://github.com/tanyazyabkina/AmazonComprehend/blob/master/Use_Amazon_Comprehend_API_GitHub_.ipynb

Additional outputs JSON to CSV
https://github.com/tanyazyabkina/AmazonComprehend/blob/master/AWS_Comprehend_JSON_to_CSV.ipynb

## Reference
### Boto3 Comrehend
https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html
### Boto3 S3
https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html

