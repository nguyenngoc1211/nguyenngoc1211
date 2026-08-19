# QUICK SETUP

## 1. Repository name

Create a **public** repository named exactly:

```text
nguyenngoc1211
```

Because your GitHub username is also `nguyenngoc1211`.

## 2. Copy everything

Extract this ZIP and copy all files into the repository, including the hidden `.github` folder.

Structure:

```text
.
├── README.md
├── SETUP.md
├── assets
│   ├── hero.svg
│   ├── operations.svg
│   └── footer.svg
└── .github
    └── workflows
        └── snake.yml
```

## 3. Push

```bash
git add .
git commit -m "feat: redesign github profile"
git push origin main
```

## 4. Run the snake once

Go to:

```text
Repository
→ Actions
→ Contribution Snake
→ Run workflow
```

If Actions cannot push the generated `output` branch:

```text
Settings
→ Actions
→ General
→ Workflow permissions
→ Read and write permissions
→ Save
```

Then rerun the workflow.

## 5. Pin these repositories

Recommended order:

1. web-threat-early-warning
2. threat_hunter_APT
3. WU-CTF
4. ma_lai_RSA_va_AES_ung_dung_ma_hoa_email

Then choose your two best remaining repositories.

## 6. Suggested GitHub bio

```text
Cybersecurity Student @ PTIT
SOC | Threat Detection | Threat Hunting | CTF
```

## 7. Design language

This version intentionally avoids the “gaming hacker dashboard” look.

Palette:

```text
Background      #090B10
Primary cyan    #7DE7FF
Violet          #A78BFA
Pink accent     #FF5C9A
Text            #F8FAFC
Muted text      #94A3B8
```

The hero and project cards are custom local SVG assets, so the profile has a consistent visual identity rather than looking like a generic README generator.
