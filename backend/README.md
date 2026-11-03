# PhoyaniMap Backend

Minimal Go HTTP server (standard library only) to connect the frontend to later.

## Run

```bash
cd backend
go run .
```

Server starts on `http://localhost:8080` (override with `PORT`).

## Endpoints

| Method | Path          | Description          |
| ------ | ------------- | -------------------- |
| GET    | `/api/health` | Liveness check       |
| GET    | `/api/hello`  | Example JSON endpoint |

CORS is open (`*`) so the Vite dev server can call it during development.

## Note

Requires Go 1.22+ (uses method-based `ServeMux` routing). Go is not yet
installed on this machine — install from https://go.dev/dl/ to run.
