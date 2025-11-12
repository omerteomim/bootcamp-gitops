# Bootcamp gitops

This repository contains the GitOps configurations of the bootcamp project. The application code for the Psychometry App. is located in the [bootcamp-project](https://github.com/omerteomim/bootcamp-project) repository, and the infrastructure code are in the [bootcamp-infra](https://github.com/omerteomim/bootcamp-infra) repository.


## GitOps

This repository is designed to manage application deployments across various environments (development, staging, production) using GitOps principles. It leverages tools like Argo CD (indicated by `applicationset.yaml`) to automate the synchronization of desired application states defined in Git with the actual state in Kubernetes clusters.

## Structure

- `environments/`: Contains environment-specific configurations.
  - `applicationset.yaml`: Defines ApplicationSet resources for Argo CD, enabling the management of multiple applications from a single Git repository.
  - `dev/`: Development environment specific `values.yml` files.
  - `staging/`: Staging environment specific `values.yml` files.
  - `prod/`: Production environment specific `values.yml` files.

