To create the stack, run:

```bash
aws --region us-east-1 cloudformation create-stack --stack-name vpc-test --template-body file://vpc.yaml --parameters file://values.json
```

To update an existing stack:

```bash
aws --region us-east-1 cloudformation update-stack --stack-name vpc-test --template-body file://vpc.yaml --parameters file://values.json
```

To delete an existing stack:

```bash
AWS_PROFILE=luminar aws --region us-east-1 cloudformation delete-stack --stack-name vpc-test
```