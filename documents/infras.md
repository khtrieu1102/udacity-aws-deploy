# Udagram Infrastructure details:

# AWS Elastic Beanstalk

- The AWS Elastic Beanstalk service hosts the application server, which extracts and launches the application from an S3 bucket that has been built, archived, and uploaded there.

- Elastic Beanstalk URL: http://udagram-api-dev.us-east-1.elasticbeanstalk.com

# AWS Relational Database Service (RDS)

- Using the `postgre SQL` service to hold the database.
- Database host URL: `database-2.cxhthoi9keq4.us-east-1.rds.amazonaws.com`
- Database name: `postgres`
- Database username/password: `postgres/postgres`

# AWS S3 Bucket

- Here is the place that Frontend application Udagram have been deployed. After being built by the pipeline, the bundled javascript packages have been pushed to S3 at the URL: http://trieunnk-project-431044761649.s3-website-us-east-1.amazonaws.com/

