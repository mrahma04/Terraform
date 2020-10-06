- Create/update a shared credentials file in ~/.aws/credentials

```
[default]
aws_access_key_id = 
aws_secret_access_key = 
[terraform]
aws_access_key_id = 
aws_secret_access_key =
```

- Reference this in the Provider section

```
provider "aws" {
    region = "us-east-1"
    shared_credentials_file = "/Users/xxx/.aws/credentials"
    profile = "terraform"
}
```