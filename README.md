# master-thesis-gitops
This is the Gitops-Repo for my master thesis "A Lightweight Experimental Approach to Measure the Antifragility of Cloud-based Systems".

With [ArgoCD](argoproj.github.io/) this GitOps repository can be used to deploy the following applications to a kubernetes cluster:

- bank-of-anthos
- cadvisor
- elasticsearch
- fluentd
- grafana
- kibana
- linkerd
- linkerd-viz
- litmus
- prometheus
- A debug pod

The structure follows the [app-of-apps pattern](https://argo-cd.readthedocs.io/en/stable/operator-manual/cluster-bootstrapping/).

The `main` branch is the default setup, and the `ha-version` branch uses a different configuration for bank-of-anthos which includes changes to the pod lifecycle as well as a horizontal pod autoscaler.
