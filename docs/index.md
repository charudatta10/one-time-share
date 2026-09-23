# one-time-share docs

One Time File Sharing — upload a file and share a download link that expires
after a single download.

## Overview

A lightweight Flask web app for one-time file sharing. Files are uploaded and
encrypted, and the generated download link can only be used a single time
before the file is removed, keeping shared files private and ephemeral.

## Features

- Single-download file sharing
- Encrypted storage
- Registration / login via the web UI

## Quickstart

```bash
pip install -r requirements.txt
python run.py
```

The app listens on port 8080 by default.

## Usage

1. Register or log in at the web UI.
2. Upload a file through the upload page.
3. Share the generated single-download link with your recipient.

## Testing

```bash
python -m unittest discover -s tests
```

## Repository layout

- `src/` — Flask application
- `run.py` — server entry point
- `uploads/` — uploaded file storage (ignored by git)
- `_archive/pulse/` — merged P2P WebRTC chat + file transfer repo

## See also

- Main project [README](../README.md)
- [Changelog](../CHANGELOG.md)