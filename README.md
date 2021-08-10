# Local-stack Study
In this study project I'm using local-stack to **emulate an AWS environment locally**.

I'm also using `Docker` to make things easie to set-up, without any further software installation.

## AWS Services emulated
* IAM
* S3
* SNS
* SQS

## To set-up the environment
Just run `docker-compose up`

## To check if everything is running
Url: http://localhost:4566/health.\
You should see a result like this:
```json
  {
    "services": 
    {
      "s3": "running", 
      "sns": "running", 
      "sqs": "running", 
      "iam": "running"
    }, 
    "features": 
    {
      "persistence": "disabled", 
      "initScripts": "initialized"
    }
  }
```

