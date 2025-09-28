# K8S GitOps Reference

This repository contains Kubernetes manifests and configurations for managing deployments, secrets, and other resources using GitOps workflows.

## Contents

- **Deployments**: YAML files for application deployments.
- **Secrets**: Encrypted secrets managed via tools like Sealed Secrets or SOPS.
- **ConfigMaps**: Application configuration stored as ConfigMaps.
- **Helm Charts**: Optional Helm charts for templated deployments.

## GitOps Workflow

1. **Version Control**: All changes are tracked in Git.
2. **Automation**: Tools like ArgoCD or Flux monitor the repository and apply changes to the cluster.
3. **Auditability**: Every change is logged and reviewable.

## Usage

1. Fork or clone this repository.
2. Update manifests as needed.
3. Commit and push changes.
4. GitOps operator applies changes to the cluster.

## Best Practices

- Store secrets securely (use encryption).
- Use descriptive commit messages.
- Review changes via pull requests.

## References

- [Kubernetes Documentation](https://kubernetes.io/docs/)
- [ArgoCD](https://argo-cd.readthedocs.io/)
- [Flux](https://fluxcd.io/)
- [Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets)