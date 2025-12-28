# 📦 Helm Charts

A collection of Helm charts and Kubernetes deployment templates for packaging, configuring, and deploying applications on Kubernetes using Helm, the Kubernetes package manager. 
GitHub

# 📌 About

Helm is a tool that streamlines installing and managing Kubernetes applications by using charts — packaged collections of Kubernetes resources defined using templates. Charts allow developers and operators to define, version, share, and update applications consistently across clusters and environments. 
GitHub

This repository contains reusable Helm charts (and related configuration) for your microservices, middleware, or infrastructure components that can be installed via a simple helm install command.


# 🚀 Why Use Helm

Package Management for Kubernetes — Helm is like apt/yum/homebrew for Kubernetes. 
GitHub

Templating & Configuration — Customize deployments using parameterized values. 
GitHub

Versioned Releases — Manage application versions and rollbacks. 
GitHub

Reusable Infrastructure — Share charts across teams or host your own chart repository. 
Helm

# 🛠 Prerequisites

Ensure you have the following installed:

✔ Helm CLI (v3 or later) — to package and install charts.
✔ kubectl — to interact with your Kubernetes cluster.
✔ A running Kubernetes cluster (e.g., EKS, GKE, Minikube, Kind) configured in your kubeconfig.

# 📦 Basic Usage
Install a chart
helm install <release-name> ./<chart-directory>


Example (from local chart):

helm install myapp ./mychart

Update repository and search

If you host charts in a remote repository:

helm repo add myrepo <repo-url>
helm repo update
helm search repo mychart

# 📈 Chart Development
Create a new chart
helm create <chart-name>


This generates a scaffold with sample templates and values.

Package a chart
helm package <chart-name>


This creates a .tgz chart package.

Hosting a chart repo

Convert this repo into a Helm chart repository by generating an index.yaml and hosting the packaged charts:

helm repo index .


Then host this folder through GitHub Pages or another HTTP server. 
Helm

# 📌 Best Practices

✔ Use values.yaml to define defaults and allow overrides.
✔ Modularize charts for reuse across environments.
✔ Version charts following semantic versioning.
✔ Integrate with CI/CD pipelines for automated packaging and publishing. 
Helm

# 🤝 Contributing

Contributions are welcome! You can help by:

Adding new Helm charts

Improving existing templates

Documenting installation and configuration examples

To contribute:

Fork the repository

Create a feature branch

Commit your changes

Open a Pull Request
