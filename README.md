# Realm9 Documentation Hub

> Complete Documentation and API Reference for the Realm9 Platform

[![Docs](https://img.shields.io/badge/docs-latest-blue)](https://docs.realm9.app)
[![API](https://img.shields.io/badge/API-v1-green)](https://api.realm9.app)
[![Status](https://img.shields.io/badge/status-live-brightgreen)](https://status.realm9.app)

## Overview

Welcome to the Realm9 documentation repository. This comprehensive resource contains everything you need to deploy, configure, and manage the Realm9 platform.

## Documentation Structure

```
realm9-docs/
├── getting-started/     # Quick start guides
├── platform/           # Platform architecture and concepts
├── api/               # REST API documentation
├── deployment/        # Deployment guides
├── integrations/      # Third-party integrations
├── security/          # Security and compliance
├── troubleshooting/   # Common issues and solutions
└── release-notes/     # Version history and updates
```

## Quick Links

### 🚀 Getting Started
- [Platform Overview](./getting-started/overview.md)
- [Quick Start Guide](./getting-started/quickstart.md)
- [Installation](./deployment/installation.md)
- [First Environment](./getting-started/first-environment.md)

### 📖 Core Documentation
- [Environment Management](./platform/environments.md)
- [Terraform Integration](./platform/terraform.md)
- [RO9 Observability](./platform/observability.md)
- [Multi-Cloud Setup](./platform/multi-cloud.md)

### 🔌 API Reference
- [Authentication](./api/authentication.md)
- [Environments API](./api/environments.md)
- [Bookings API](./api/bookings.md)
- [Terraform API](./api/terraform.md)
- [Webhooks](./api/webhooks.md)

### 🛠️ Administration
- [User Management](./admin/users.md)
- [RBAC Configuration](./admin/rbac.md)
- [Backup & Recovery](./admin/backup.md)
- [Monitoring](./admin/monitoring.md)

## Platform Guides

### Environment Management
Complete guide to managing environments including:
- Creating and configuring environments
- Booking and approval workflows
- Cost tracking and chargeback
- Shared environment management
- Maintenance windows

### Infrastructure Automation
- Natural language to Terraform
- GitOps workflows
- Policy as code
- Drift detection
- Cost optimization

### Observability (RO9)
- Log ingestion setup
- Query optimization
- Dashboard creation
- Alert configuration
- Data retention policies

### Security & Compliance
- MFA setup
- SSO configuration
- Audit logging
- Compliance reporting
- Security best practices

## Integration Guides

### CI/CD
- [GitHub Actions](./integrations/github-actions.md)
- [GitLab CI](./integrations/gitlab-ci.md)
- [Jenkins](./integrations/jenkins.md)
- [Azure DevOps](./integrations/azure-devops.md)

### ITSM
- [ServiceNow](./integrations/servicenow.md)
- [Jira Service Management](./integrations/jira.md)
- [PagerDuty](./integrations/pagerduty.md)

### Cloud Providers
- [AWS Setup](./integrations/aws.md)
- [Azure Configuration](./integrations/azure.md)
- [GCP Integration](./integrations/gcp.md)
- [VMware vSphere](./integrations/vmware.md)

## Deployment Options

### ☁️ Cloud (SaaS)
Fastest way to get started:
```bash
curl -X POST https://api.realm9.app/signup \
  -H "Content-Type: application/json" \
  -d '{"organization": "your-org"}'
```

### 🏢 Self-Hosted
Full control in your infrastructure:
- [Kubernetes Deployment](./deployment/kubernetes.md)
- [Docker Compose](./deployment/docker.md)
- [Air-Gap Installation](./deployment/airgap.md)
- [High Availability](./deployment/ha.md)

## API Examples

### Environment Creation
```bash
curl -X POST https://api.realm9.app/v1/environments \
  -H "Authorization: Bearer $TOKEN" \
  -H "Content-Type: application/json" \
  -d '{
    "name": "prod-app-01",
    "type": "PRODUCTION",
    "cloud": "AWS",
    "region": "us-east-1"
  }'
```

### Terraform Execution
```bash
curl -X POST https://api.realm9.app/v1/terraform/run \
  -H "Authorization: Bearer $TOKEN" \
  -d '{
    "workspace": "production",
    "action": "apply",
    "auto_approve": false
  }'
```

## Troubleshooting

### Common Issues
- [Authentication Errors](./troubleshooting/auth.md)
- [Terraform Failures](./troubleshooting/terraform.md)
- [Performance Issues](./troubleshooting/performance.md)
- [Network Problems](./troubleshooting/network.md)

### Debug Tools
```bash
# Check system status
realm9 status --verbose

# Validate configuration
realm9 config validate

# Test connectivity
realm9 test connection --all

# Generate support bundle
realm9 support bundle --output realm9-debug.tar.gz
```

## Release Notes

### Latest Version (v2.5.0)
- ✅ AI-powered infrastructure co-pilot
- ✅ RO9 observability platform GA
- ✅ ServiceNow CMDB integration
- ✅ Multi-cloud cost analysis
- ✅ Enhanced security features

[View all releases →](./release-notes/)

## Migration Guides

### From Other Platforms
- [Migrating from Enov8](./migration/from-enov8.md)
- [Migrating from Plutora](./migration/from-plutora.md)
- [Migrating from Terraform Cloud](./migration/from-terraform-cloud.md)

## Video Tutorials

- 🎥 [Platform Overview](https://videos.realm9.app/overview) (10 min)
- 🎥 [Getting Started](https://videos.realm9.app/getting-started) (15 min)
- 🎥 [Terraform Integration](https://videos.realm9.app/terraform) (20 min)
- 🎥 [RO9 Observability](https://videos.realm9.app/observability) (25 min)

## Community & Support

### Resources
- **Forum**: [community.realm9.app](https://community.realm9.app)
- **Slack**: [realm9.slack.com](https://realm9.slack.com)
- **Stack Overflow**: [#realm9](https://stackoverflow.com/tags/realm9)

### Support Channels
- **Documentation**: You are here!
- **Community Support**: GitHub Discussions
- **Professional Support**: support@realm9.app
- **Enterprise Support**: 24/7 with SLA

## Contributing

We welcome contributions to our documentation:

1. Fork this repository
2. Create a feature branch
3. Make your improvements
4. Submit a pull request

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## License

Copyright © 2025 Realm9. All rights reserved.

---

**Need help?** Contact [support@realm9.app](mailto:support@realm9.app) or visit [realm9.app/support](https://realm9.app/support)

Part of the [Realm9 Platform](https://github.com/realm9-platform/realm9)
