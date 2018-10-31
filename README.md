# terraform-bucket-initializer

Script of creation S3 bucket for Terraform backend.

## Description

Terraform is an administrative tool that manages your infrastructure,
and so ideally the infrastructure that is used by Terraform should exist
outside of the infrastructure that Terraform manages.

So, this script provision S3 bucket for Terraform backend, which provides recommended settings.

- Enable Default Encryption
- Enable Versioning

## Requirements

- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html)

## Usage

```sh
curl -fsSL https://raw.githubusercontent.com/tmknom/terraform-bucket-initializer/master/init | sh -s <bucket_name> <region>
```

## Makefile targets

```text
format                         Format code
help                           Show help
install                        Install requirements
lint                           Lint code
```

## License

Apache 2 Licensed. See LICENSE for full details.
