# gitops-cookbook

Collection of projects based on GitOps approach

![](https://i.imgur.com/0BR0O7y.png)


## What is GitOps?

[**GitOps**](https://www.atlassian.com/git/tutorials/gitops) is a modern DevOps approach where **Git is the single source of truth** for infrastructure and application deployment.

- You **store all configuration and deployment code** (e.g., Kubernetes manifests, Terraform files) in a **Git repository**.
- Any change (infra or app) is done via a **Git commit + pull request**.
- A **GitOps operator** (like ArgoCD or Flux) **automatically syncs** the live system with the Git repo by using **orchestrator** such as **Kubernetes**
- If the actual state drifts from the desired state in Git, the system will **reconcile it automatically**.

![](./img/gitops_workflow.png)

### Key Benefits:
- **Version control** for everything
- **Auditability** (you know who changed what and when)
- **Automation** (CI/CD pipelines and auto-sync)
- **Rollback** by reverting a Git commit

## Projects
- [Demo of deploying Flux operator into Minikube cluster and connecting it to the Github repository](https://github.com/Brain2life/flux-demo)

## References
- [O'Reilly GitOps Cookbook repository: github.com/gitops-cookbook](https://github.com/gitops-cookbook)