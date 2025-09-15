[README.md](https://github.com/user-attachments/files/22350761/README.md)
# RefTrack Lite (Web MVP)

**Referral → SMS templates** in seconds. Upload a PDF, get professional/friendly/neutral messages for RingCentral.

## Quick Start (Docker)
```bash
docker build -t reftrack-lite .
docker run -it --rm -p 8000:8000 -e REFTRACK_API_KEY=derma123 reftrack-lite
```
Open `frontend/index.html` → set API URL `http://localhost:8000` and API Key `derma123`.

## Endpoints
- `GET /api/health`
- `POST /api/process` (form field: `file` as PDF)

## Security
Set `REFTRACK_API_KEY` and pass it as `x-api-key` header from the frontend.

# 🚀 One-Click Deploy (Render)

After you push this repo to **GitHub**, click this link (replace `YOUR_GITHUB_REPO_URL` with your repo URL):

**Deploy to Render:**  
https://render.com/deploy?repo=YOUR_GITHUB_REPO_URL

> Example: if your repo is `https://github.com/yourname/reftrack-lite-web`, use:  
> https://render.com/deploy?repo=https://github.com/yourname/reftrack-lite-web

Render will auto-detect the **Dockerfile** and spin up your API at a URL like:  
`https://reftrack-lite.onrender.com`
