# Hacking-ToolsBug Bounty Toolkit - Web & API + Mobile (Android/iOS)
Repository List (Generated: 22 January 2026 (Asia/Jakarta)) By – MR0615

Disclaimer: Use this tool only for permitted (in-scope) testing and in accordance with the policies of the bug bounty program you are participating in.

https://docs.google.com/document/d/1YLUglZ8sCXBukEPPnnz8iFgrrVESEx8NvAWBM8tFk44/edit?usp=sharing


# Bug Bounty Daily Workflow (Web/API + Mobile)

> Gunakan hanya pada aset **in-scope** dan patuhi **Program Policy** serta **HackerOne Code of Conduct**. :contentReference[oaicite:1]{index=1}  
> Report yang baik harus punya: **judul jelas, langkah reproduksi rinci, bukti/PoC, dan impact**. :contentReference[oaicite:2]{index=2}  
> Video PoC bisa membantu memperjelas dan HackerOne mendukung perekaman PoC. :contentReference[oaicite:3]{index=3}

---

## 0) Struktur Folder (Repo Layout)

bugbounty-workflow/
├─ README.md
├─ programs/
│ └─ <program_name>/
│ ├─ 00-scope/
│ │ ├─ in-scope.txt
│ │ ├─ out-of-scope.txt
│ │ └─ notes.md
│ ├─ 01-recon/
│ │ ├─ subdomains.txt
│ │ ├─ live_hosts.txt
│ │ ├─ ports.txt
│ │ ├─ crawled_urls.txt
│ │ ├─ wayback_urls.txt
│ │ └─ nuclei_findings.txt
│ ├─ 02-validation/
│ │ ├─ repro_steps.md
│ │ ├─ requests/
│ │ └─ evidence/
│ ├─ 03-mobile/
│ │ ├─ binaries/
│ │ ├─ static/
│ │ ├─ dynamic/
│ │ └─ traffic/
│ ├─ 04-reports/
│ │ ├─ draft.md
│ │ ├─ final.md
│ │ └─ attachments/
│ └─ 99-archive/
├─ templates/
│ ├─ report_template_h1.md
│ ├─ repro_template.md
│ └─ triage_checklist.md
└─ scripts/
├─ web_recon.sh
├─ web_crawl.sh
├─ web_scan.sh
└─ mobile_notes.sh

