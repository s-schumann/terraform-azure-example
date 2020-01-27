# Azure Terraform Skeleton

## Service Description

This skeleton spins up a small instance in the West Europe region of the hyperscaler Microsoft Azure. It creates all prerequisites (e.g. resource group, networking, DNS zone).

Set the variables in the `terraform.tfvars` file and apply the configuration (see below).

To log into Microsoft Azure, Terraform provides the possibility to use the command line tool `az`.

It can be installed on macOS using `brew install azure-cli` [1].

Use `az login` to log in via the browser[2].

## Usage

```bash
$ terraform init
```

```bash
$ ( export TF_VAR_domain="test.example.com"; export TF_VAR_public_key="ssh-ed25519 AAAA..."; terraform apply )
```

## Notes and References

Parts of this script follow [3].

[1] https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-macos?view=azure-cli-latest

[2] https://www.terraform.io/docs/providers/azurerm/guides/azure_cli.html

[3] https://learn.hashicorp.com/terraform/azure/dependencies_az

# Version

* Version 0.0.1

# Contact

Copyright (c) 2020 Sebastian Schumann

* E-mail: [mail@s-schumann.com](mailto:mail@s-schumann.com "mail to sebastian")
* Homepage: [www.s-schumann.com](https://s-schumann.com "my website")

# License

The software is licensed under the [MIT LICENSE](LICENSE)
