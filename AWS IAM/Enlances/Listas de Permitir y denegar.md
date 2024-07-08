**Lista de permitir**
```
{
"version": "2012-10-17",
"Statement":[
		{
			"Effect": "Allow",
			"Action": [
			"ecs:*",
			"cloudwatch:*"
			],
			"Resource":"*"
		}
	]
}
```
Lista de denegar
```
{
	"Version": "2012-10-17",
	"Statement": [
		{
			"Sid": "AllowsAllActions",
			"Effect":"Allow",
			"Action":"*",
			"Resource":"*"
		},
		{
			"Sid": "DenyDynamoDB",
			"Effect":"Deny",
			"Action":"dynamodb:*",
			"Resource":"*"
		}
	]
}
```