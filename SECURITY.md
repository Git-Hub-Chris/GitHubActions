# Security Policy

## Supported Versions

Versions are currently being supported with security updates.

| Version | Supported          |
| ------- | ------------------ |
| 5.1.x   | :white_check_mark: |
| 5.0.x   | :x:                |
| 4.0.x   | :white_check_mark: |
| < 4.0   | :x:                |

## Reporting a Vulnerability

We take security seriously and appreciate your help in identifying and fixing vulnerabilities. Please report security vulnerabilities responsibly by emailing security@example.com instead of using the public issue tracker.

### Reporting Process

1. **Email the security team** with details about the vulnerability
2. **Do not disclose** the vulnerability publicly until we've had time to address it
3. **Include a proof-of-concept** or steps to reproduce if possible
4. **Allow 90 days** for us to develop and release a fix before public disclosure

We aim to respond to security reports within 7 days and provide an update on our progress within 30 days.

## Security Best Practices for GitHub Actions

### For Contributors

- **Review workflows carefully** - Only approve pull requests that modify workflows after thorough review
- **Use pinned actions** - Always pin actions to a specific commit SHA, not floating tags
- **Avoid hardcoded secrets** - Never commit secrets or credentials; use GitHub Secrets
- **Validate inputs** - Sanitize all external inputs in workflows to prevent injection attacks
- **Keep dependencies updated** - Regularly update action versions and dependencies for security patches
- **Use CODEOWNERS** - Require approval from code owners for workflow changes

### For Users

- **Review workflows before using** - Audit any GitHub Actions workflows before running them
- **Monitor for updates** - Subscribe to security advisories for actions you use
- **Limit permissions** - Use the principle of least privilege for workflow permissions
- **Audit logs** - Regularly review workflow runs and audit logs for suspicious activity
- **Environment protection** - Use environment protection rules for sensitive deployments

## Security Features in This Repository

- ✅ **Required commit signatures** - Commits are signed
- ✅ **Workflow approval** - Changes to workflows require approval
- ✅ **Dependabot monitoring** - Automated vulnerability scanning enabled
- ✅ **Branch protection rules** - Main branch is protected from direct pushes
- ✅ **MIT License** - Full transparency of code and usage

## Dependencies and Vulnerability Scanning

This repository uses the following security measures:

- GitHub's native dependency vulnerability scanning
- Pre-commit hooks for code quality
- Automated testing and validation

## Security Contact

For security concerns, please contact:
- **Email**: security@example.com
- **Response time**: Within 7 business days

## Disclaimer

While we strive to maintain the security of this project, no software is completely secure. Users are responsible for implementing appropriate security measures when using GitHub Actions in their workflows and environments.