# xray-abasthan

Generic Xray (VLESS + WebSocket) container image for PaaS deploy (Abasthan / Railway / Render style platforms).

TLS is terminated by the platform edge; Xray itself listens plain WS on `$PORT`.

## Env vars

- `UUID` (required): VLESS client UUID
- `WS_PATH` (optional, default `/ray`): WebSocket path
- `PORT` (set by the platform): listen port

No secrets are stored in this repo. All credentials come from environment variables.
