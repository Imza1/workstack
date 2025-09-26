# Copilot Instructions

## General

- Ask clarifying questions when inputs are ambiguous; do not guess.
- Do not invent facts; if you assume, say so in a comment.
- Prefer small, readable functions and PEP8 naming.

## Definitions & Explanations

- When asked for a definition, give a 1–2 sentence explanation and a tiny example.
- If trade-offs exist, list the top 2 briefly.

## Terraform

- Pin provider versions and Terraform version.
- Generate code that passes: `terraform fmt`, `terraform validate`.
- Prefer modules only when it reduces duplication; otherwise keep it simple.

## Python

- Follow PEP8; include type hints where trivial.
- Use docstrings with a short usage example when writing functions/CLIs.

## Linux

- Use shell scripting to automate repetitive tasks.
- Follow best practices for writing portable and maintainable shell scripts.
- Prefer `bash` or `zsh` for scripting; include comments for clarity.
- Use tools like `grep`, `awk`, and `sed` for text processing.

## Security

- Do not output secrets or credentials.
- For AWS, suggest using aws-vault / env vars; avoid plaintext creds.

## When Unsure

- Ask one clarifying question before proceeding.

## AWS

- Use `aws-vault` or environment variables to manage credentials securely.
- Prefer Infrastructure as Code (IaC) tools like Terraform or AWS CloudFormation.
- Automate deployments using AWS CLI, SDKs (e.g., `boto3`), or CI/CD pipelines.
- Follow the principle of least privilege when creating IAM roles and policies.

## Git

- Use meaningful commit messages (e.g., "Add feature X" instead of "Fix bug").
- Follow a branching strategy (e.g., Git Flow, trunk-based development).
- Regularly rebase or merge to keep branches up-to-date.
- Use `.gitignore` to exclude unnecessary files from version control.
- Use virtual environments (`venv` or `poetry`) to manage dependencies.
- Write Python scripts for automation (e.g., file management, API calls).
- Use logging instead of `print` for better debugging and monitoring.

## Learning Resources

- **Python**: [Real Python](https://realpython.com), [Automate the Boring Stuff](https://automatetheboringstuff.com)
- **Linux**: [Linux Journey](https://linuxjourney.com), [The Linux Command Line](https://linuxcommand.org)
- **Terraform**: [Terraform Docs](https://developer.hashicorp.com/terraform/docs), [Learn Terraform](https://learn.hashicorp.com/terraform)
- **AWS**: [AWS Training](https://aws.amazon.com/training), [AWS Well-Architected Framework](https://aws.amazon.com/architecture/well-architected)
- **Git**: [Pro Git](https://git-scm.com/book/en/v2), [GitHub Docs](https://docs.github.com)

## CI/CD

- Use tools like GitHub Actions, Jenkins, or GitLab CI/CD for automation.
- Write pipelines to automate testing, building, and deployment.
- Ensure pipelines are idempotent and fail gracefully.
