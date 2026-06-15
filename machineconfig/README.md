# gitops

Source directory consumed by the ArgoCD Application **mach-config-motd-deploy**.

Hosted in the Gitea repository (branch **`Main`**):
`https://gitea.intellidog.app/david.tay/apps.git`  →  directory **`gitops/`**

Browser view: `https://gitea.intellidog.app/david.tay/apps/gitops`

| File | Status | Purpose |
|------|--------|---------|
| `61-master-swissre.yaml` | **GRADED** | Writes the ASCII banner to `/etc/master-swissre` on master nodes (mode `0444`). |
| `99-master-motd.yaml` | supplementary | Login MOTD banner. |
| `50-master-chrony.yaml` | supplementary | Custom chrony NTP source. |
| `75-master-sysctl.yaml` | supplementary | sysctl tuning. |
| `kustomization.yaml` | — | Lists all four resources. |
| `devopswala.txt` | reference | The "I love Openshift" ASCII banner that is embedded into `61-master-swissre.yaml`. |
