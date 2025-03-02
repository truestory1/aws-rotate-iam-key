# Ansible Role: Rotate AWS IAM User Keys

This Ansible role is designed to rotate AWS IAM user keys. It ensures that the keys are rotated regularly to maintain security and compliance.

## Requirements

None.

## Role Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `aws_access_key` | AWS access key ID | `""` |
| `aws_secret_key` | AWS secret access key | `""` |
| `iam_user` | IAM user whose keys are to be rotated | `""` |

## Dependencies

None.

## Example Playbook

```yaml
- hosts: localhost
  roles:
    - role: rotate-aws-iam-user-keys
      aws_access_key: YOUR_AWS_ACCESS_KEY
      aws_secret_key: YOUR_AWS_SECRET_KEY
      iam_user: YOUR_IAM_USER
```

