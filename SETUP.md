# SETUP — CLASSIFIED SOC DOSSIER

This version is intentionally very different from the earlier neon/cyberpunk profile.

## Visual direction

- Black / dark charcoal
- Classified dossier red
- Amber radar signal
- Military/SOC case-file layout
- No purple/cyan cyberpunk cards
- No giant wall of badges
- Custom SVG visuals stored locally

## Repository structure

```text
.
├── README.md
├── SETUP.md
├── assets
│   ├── classified-header.svg
│   ├── radar-console.svg
│   ├── case-files.svg
│   ├── capabilities.svg
│   └── footer-stamp.svg
└── .github
    └── workflows
        └── snake.yml
```

## Push

```bash
git add .
git commit -m "feat: switch profile to classified SOC dossier"
git push origin main
```

## Contribution trace

After push:

```text
GitHub → Actions → Contribution Trace → Run workflow
```

If it cannot publish:

```text
Settings → Actions → General
→ Workflow permissions
→ Read and write permissions
```

## Suggested pinned repositories

1. web-threat-early-warning
2. threat_hunter_APT
3. WU-CTF
4. ma_lai_RSA_va_AES_ung_dung_ma_hoa_email

## Suggested profile bio

```text
Cybersecurity Student @ PTIT
SOC • Threat Detection • Threat Hunting • CTF
```
