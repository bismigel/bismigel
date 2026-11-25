Senior observability & platform engineer in Toronto. I run a three-node Kubernetes cluster at home, where fenced
AI agents diagnose alerts.

**[Cluster desired state](https://github.com/bismigel/bakuran-gitops)** — about 50 ArgoCD Applications on k3s. Every
one of the 81 alert rules has a runbook entry generated from the rules; CI checks the manifests, image digests,
alert-to-runbook links and image scans, and a CVE baseline fails on anything new. Alert agents talk A2A and are held
by read-only tools, RBAC and an admission policy.

**[Infrastructure](https://github.com/bismigel/bakuran-infra)** — NixOS hosts, OpenTofu for the router and firewall,
Ansible, and a staging VM where network changes are rehearsed before production.

**[orchestra](https://github.com/bismigel/orchestra)** — a strong model decides, cheap sandboxed models type. Workers
implement settled specs in their own worktree; every result is reviewed and proven on the exact code before it lands.
44 measured runs: 121M tokens, $3.08 in total.

**[Datadog docs fix](https://github.com/DataDog/documentation/pull/41325)** — corrected the HashiCorp Vault
`implicit_auth` reference after reproducing an Agent 7.85.0 startup failure; approved by the Datadog docs team.
The integration behind it: [Helm chart](https://github.com/bismigel/datadog-vault-k8s-template) ·
[Docker/Podman template](https://github.com/bismigel/dd-agent-hashi-secret-template).

[bismigel.dev](https://bismigel.dev) · work@bismigel.dev
