# SETUP — NGOC // CYBER OPERATIONS PROFILE

## 1. Tạo đúng repository

Repository phải là:

```text
nguyenngoc1211/nguyenngoc1211
```

GitHub tự hiển thị `README.md` của public repository trùng username lên trang profile.

## 2. Push toàn bộ thư mục này

Nếu repository đã tạo sẵn:

```bash
git clone https://github.com/nguyenngoc1211/nguyenngoc1211.git
cd nguyenngoc1211
```

Copy **toàn bộ nội dung** trong package này vào repo, gồm cả thư mục ẩn `.github`.

Sau đó:

```bash
git add .
git commit -m "feat: launch cyber operations profile"
git push origin main
```

## 3. Snake

Không cần secret riêng.

Sau khi push:

```text
GitHub repo
→ Actions
→ Generate Contribution Snake
→ Run workflow
```

Workflow sẽ tạo branch `output`.

README đã trỏ tới:

```text
output/github-contribution-grid-snake.svg
output/github-contribution-grid-snake-dark.svg
```

Nếu repository đang chặn GitHub Actions ghi nội dung:

```text
Settings
→ Actions
→ General
→ Workflow permissions
→ Read and write permissions
→ Save
```

## 4. Live GitHub Metrics — tùy chọn nhưng nên bật

Profile đã có `github-metrics.svg` placeholder nên **push xong vẫn đẹp ngay**.

Muốn biến nó thành live telemetry, tạo GitHub Personal Access Token theo hướng dẫn của `lowlighter/metrics`, dùng quyền tối thiểu cần thiết cho dữ liệu bạn muốn hiển thị.

Sau đó vào:

```text
Repository
→ Settings
→ Secrets and variables
→ Actions
→ New repository secret
```

Tên secret:

```text
METRICS_TOKEN
```

Paste token vào.

Tiếp theo:

```text
Actions
→ GitHub Metrics
→ Run workflow
```

Workflow sẽ tự thay `github-metrics.svg` bằng telemetry thật.

## 5. Những repo nên Pin

Vào profile:

```text
Customize your pins
```

Ưu tiên:

1. web-threat-early-warning
2. threat_hunter_APT
3. WU-CTF
4. ma_lai_RSA_va_AES_ung_dung_ma_hoa_email

Sau đó thêm 2 project tốt nhất còn lại.

## 6. About profile gợi ý

```text
Cybersecurity Student @ PTIT
SOC | Threat Detection | Threat Hunting | CTF
```

## 7. Nếu muốn chỉnh màu

Các màu chính trong SVG:

```text
Neon Cyan   #00F5FF
Purple      #9D4EDD
Pink        #FF2E88
Terminal    #39FF14
Background  #050816
```

Search/replace các mã màu trong `assets/*.svg`.

## 8. Cấu trúc package

```text
.
├── README.md
├── SETUP.md
├── github-metrics.svg
├── assets
│   ├── cyber-banner.svg
│   ├── terminal.svg
│   └── mission-grid.svg
└── .github
    └── workflows
        ├── metrics.yml
        └── snake.yml
```

## Lưu ý

- Không commit Personal Access Token vào code.
- Chỉ lưu token bằng GitHub Actions Secrets.
- `METRICS_TOKEN` là tùy chọn; snake dùng `GITHUB_TOKEN` GitHub tự cấp cho workflow.
