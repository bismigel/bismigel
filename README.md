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


**[o11y-alert-tuner](https://github.com/bismigel/o11y-alert-tuner)** — a small local model plus guard rails that triage
Prometheus alerting rules (flapping, noisy, dead, healthy) and propose patches for review. On an independent simulator it
classifies 96.7% correctly against 47.9% for the untouched base model; on my cluster, 16 of 21 real alerts against 1 for
the base model and 10 for a large API model. [Write-up](https://bismigel.dev/posts/alert-triage-with-a-small-local-model/) ·
[model](https://huggingface.co/bismigel/o11y-alert-tuner-4b).

[bismigel.dev](https://bismigel.dev) · work@bismigel.dev
