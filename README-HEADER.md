# PBS TF ecr module

## Installation

### Using the Repo Source

```hcl
module "ecr" {
    source = "github.com/pbs/terraform-aws-ecr-module?ref=x.y.z"
}
```

### Alternative Installation Methods

More information can be found on these install methods and more in [the documentation here](./docs/general/install).

## Usage

This module provisions an ECR repository. It is created with an image retention policy.

Integrate this module like so:

```hcl
module "ecr" {
  source = "github.com/pbs/terraform-aws-ecr-module?ref=x.y.z"

  # Tagging Parameters
  organization = var.organization
  environment  = var.environment
  product      = var.product
  repo         = var.repo

  # Optional Parameters
}
```

## Adding This Version of the Module

If this repo is added as a subtree, then the version of the module should be close to the version shown here:

`x.y.z`

Note, however that subtrees can be altered as desired within repositories.

Further documentation on usage can be found [here](./docs).

Below is automatically generated documentation on this Terraform module using [terraform-docs][terraform-docs]

---

[terraform-docs]: https://github.com/terraform-docs/terraform-docs
