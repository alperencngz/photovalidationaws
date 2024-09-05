Lambda_API.py:

When a new object is created in S3 with an image in it,
S3 sends signal to Lambda,
Lambda takes the image and sends it to Rekognition to do evaluations,
According to our parameters Lambda determines if it is a pass or fail (for a passaport picutre),
Lambda stores the information in DynamoDB,
Sends and SNS signal to inform subscribers about the new image and its conditions.

DynamoDB.py:

Creates an API for our DynamoDB database,
If called returns the information about certain image.

Project details :

[https://onyx-pint-13d.notion.site/Recognition-Project-AWS-64ab84275e6d4f6fa007c5feb4a7c874](https://onyx-pint-13d.notion.site/GitHub-explanation-75153456d7d643cea49ee2829434d259?pvs=4)
