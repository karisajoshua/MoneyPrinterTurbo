# MoneyPrinterTurbo Web

Vercel-hosted control plane for MoneyPrinterTurbo.

## Architecture

The web application does not run FFmpeg, MoviePy, Whisper, or long-running render jobs. Those remain in a dedicated worker service. The web layer will submit jobs, display status, and expose generated assets.

## Local development

```bash
cd web
npm install
npm run dev
```

For Vercel, configure the project Root Directory as `web`.
