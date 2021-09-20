# terraform-aws-public-route53-zone

[![Terraform Version](https://img.shields.io/badge/Terraform%20Version->=0.12.0,<0.13.0-blue.svg)](https://releases.hashicorp.com/terraform/)
[![Release](https://img.shields.io/github/release/traveloka/terraform-aws-public-route53-zone.svg)](https://github.com/traveloka/terraform-aws-public-route53-zone/releases)
[![Last Commit](https://img.shields.io/github/last-commit/traveloka/terraform-aws-public-route53-zone.svg)](https://github.com/traveloka/terraform-aws-public-route53-zone/commits/master)
[![Issues](https://img.shields.io/github/issues/traveloka/terraform-aws-public-route53-zone.svg)](https://github.com/traveloka/terraform-aws-public-route53-zone/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/traveloka/terraform-aws-public-route53-zone.svg)](https://github.com/traveloka/terraform-aws-public-route53-zone/pulls)
[![License](https://img.shields.io/github/license/traveloka/terraform-aws-public-route53-zone.svg)](https://github.com/traveloka/terraform-aws-public-route53-zone/blob/master/LICENSE)
![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.png?v=103)

## Description

Terraform module to create a public Route53 hosted zone

## Table of Content

* [terraform-aws-public-route53-zone](#terraform-aws-public-route53-zone)
   * [Description](#description)
   * [Table of Content](#table-of-content)
   * [Prerequisites](#prerequisites)
   * [Dependencies](#dependencies)
   * [Terraform Version](#terraform-version)
   * [Requirements](#requirements)
   * [Providers](#providers)
   * [Modules](#modules)
   * [Resources](#resources)
   * [Inputs](#inputs)
   * [Outputs](#outputs)
   * [Contributing](#contributing)
   * [License](#license)

## Prerequisites

This module doesn't have any existing resource requirements

## Dependencies

Doesn't have any dependencies to any other Terraform module

## Terraform Version

This module was created using Terraform `0.11.14`
The latest stable version of Terraform which this module tested working is Terraform `0.12.31` on 2021/09/17

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_route53_zone.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route53_zone) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_delegation_set_id"></a> [delegation\_set\_id](#input\_delegation\_set\_id) | The delegation set ID whose NS records will be assigned the hosted zone | `string` | `""` | no |
| <a name="input_environment"></a> [environment](#input\_environment) | Environment this Route 53 zone belongs to | `string` | n/a | yes |
| <a name="input_force_destroy"></a> [force\_destroy](#input\_force\_destroy) | Whether to destroy all records inside if the hosted zone is deleted | `string` | `false` | no |
| <a name="input_name"></a> [name](#input\_name) | Name of the hosted zone | `string` | n/a | yes |
| <a name="input_product_domain"></a> [product\_domain](#input\_product\_domain) | Abbreviation of the product domain this Route 53 zone belongs to | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_name_servers"></a> [name\_servers](#output\_name\_servers) | A list of name servers in associated (or default) delegation set |
| <a name="output_zone_id"></a> [zone\_id](#output\_zone\_id) | The hosted zone id |

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

## Contributing

This module accepting or open for any contributions from anyone, please see the [CONTRIBUTING.md](https://github.com/traveloka/terraform-aws-public-route53-zone/blob/master/CONTRIBUTING.md) for more detail about how to contribute to this module.

## License

This module is under Apache License 2.0 - see the [LICENSE](https://github.com/traveloka/terraform-aws-public-route53-zone/blob/master/LICENSE) file for details.