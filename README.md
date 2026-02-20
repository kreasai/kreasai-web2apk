# Builder Public Repo Template

Repo public untuk proses build Android dari input Web2APK.

## Trigger
Workflow dipanggil melalui `workflow_dispatch` dengan input:
- `job_id`
- `source_type` (`url` / `zip`)
- `source_url`
- `source_zip_path`
- `app_name`
- `package_name`
- `version_name`
- `version_code`
- `permissions`
- `features`

## Wajib Secrets (repo public)
- `WEB2APK_CALLBACK_URL`
- `WEB2APK_CALLBACK_TOKEN`

## Catatan
- Untuk mode simulasi di backend, workflow ini tidak wajib aktif.
- Untuk production, workflow ini harus kirim status ke callback backend (`running/success/failed`).
