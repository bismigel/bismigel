Three-node k3s homelab on NixOS, everything declared in git.

- **[Infrastructure](https://github.com/bismigel/bakuran-infra)** — NixOS hosts, OpenTofu for the router and firewall, Ansible, and a staging VM where network changes are rehearsed before production.
- **[Cluster desired state](https://github.com/bismigel/bakuran-gitops)** — ArgoCD. One workflow per alert, generated from the alert rules; a CVE baseline that fails CI when a new finding lands; alert-to-runbook links checked in CI.
- **[Build log](https://github.com/bismigel/bismigel-site)** — Org files to Hugo, with each incident written up while the details are still wrong.

The reasoning lives in `docs/decisions/`: why a PersistentVolumeClaim is never deleted, why a remediation engine may schedule a fix but not own it.
