# Contributing a new CVE entry

## Layout

```text
<product>/cve-<YEAR>-<NUMBER>-<short-slug>/
├── README.md
├── docs/
├── lab/
└── checker/
```

Example: `php/cve-2026-109618-php2shell/`

## Checklist

1. Copy [templates/CVE-ENTRY-README.template.md](templates/CVE-ENTRY-README.template.md) into the new entry  
2. Add a row to the **Catalog** in the root [README.md](README.md)  
3. Bind lab ports to **`127.0.0.1`** in Docker Compose  
4. Pin upstream PoCs by **URL + commit SHA**; use `fetch-vendors.sh` when possible  
5. No secrets, personal paths, video assets, or production evidence  
