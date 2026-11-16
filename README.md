Three-node k3s homelab on NixOS, everything declared in git.

**[Cluster desired state](https://github.com/bismigel/bakuran-gitops)** — ArgoCD across 29 app groups. 72 runbook
workflows generated from the alert rules, four required checks (manifest layout, image digests, alert-to-runbook links,
image scan), and a CVE baseline that fails CI on anything new.

**[Infrastructure](https://github.com/bismigel/bakuran-infra)** — NixOS hosts, OpenTofu for the router and firewall,
Ansible, and a staging VM where network changes are rehearsed before production.
