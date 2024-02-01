# kubecraft

kubecraft is a cluster manager utilizing the open source tools kind, flux and and cluster-api.

You bring your configuration in the form of a flux github repository and kubecraft does the rest.

# modules
kubecraft is split into multiple modules

### kubecraft-kind
Used to spin up a kind cluster, install flux and cluster api and sync the provided repository

### kubecraft-hetzner
Helm chart that holds cluster-api definitions to spin up a cluster on hetzner

### kubecraft-library
Library chart that holds common configuration, e.g. ghcr.io or bitnami HelmRepository for flux
