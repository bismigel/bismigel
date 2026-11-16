Three-node k3s homelab on NixOS, everything declared in git.

- **[bakuran-infra](https://github.com/bismigel/bakuran-infra)** — NixOS hosts, OpenTofu for the OPNsense router, Ansible, and a staging host where datapath changes are rehearsed before production.
- **[bakuran-gitops](https://github.com/bismigel/bakuran-gitops)** — ArgoCD desired state. One WorkflowTemplate per alert generated from the alert rules; a CVE baseline that fails CI when a new finding lands; no privileged containers.
- **[bismigel-site](https://github.com/bismigel/bismigel-site)** — the build log, written in Org, converted to Hugo.

Most of the reasoning is in `docs/decisions/` rather than in prose: why a PVC is never deleted, why a remediation engine may schedule but not own the remedy, why the git origin moved off GitHub.
