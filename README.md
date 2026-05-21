# Veeam DB Dump Tool

Local web tool to pull a `pg_dump` of a Veeam Backup appliance database (Azure / AWS / GCP) over SSH and download it as a `.zip`.

## How to start

**macOS:** double-click `start.command`
**Windows:** double-click `start.bat`

First launch creates a local Python virtual environment and installs dependencies (~1 minute, one-time). After that, the browser opens automatically to `http://127.0.0.1:8000`.

Fill in the form (platform, host, SSH credentials), click **Generate**, and the dump is downloaded to your Downloads folder. Click **Exit & clean** when done.

> macOS first launch: if you see "unverified developer", go to **System Settings → Privacy & Security → Open Anyway**, or run `xattr -dr com.apple.quarantine /path/to/db_dump_tool`.
