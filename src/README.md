---
tags:
  - component/sso-saml-provider
  - layer/software-delivery
  - provider/aws
---

# Component: `sso-saml-provider`

This component reads sso credentials from SSM Parameter store and provides them as outputs

## Usage

**Stack Level**: Regional

Use this in the catalog or use these variables to overwrite the catalog values.

```yaml
components:
  terraform:
    sso-saml-provider:
      settings:
        spacelift:
          workspace_enabled: true
      vars:
        enabled: true
        ssm_path_prefix: "/sso/saml/google"
```

[<img src="https://cloudposse.com/logo-300x69.svg" height="32" align="right"/>](https://cpco.io/homepage?utm_source=github&utm_medium=readme&utm_campaign=cloudposse-terraform-components/aws-sso-saml-provider&utm_content=)
