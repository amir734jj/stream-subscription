# Stream Subscription

Docker Compose setup for running the stream subscription API and UI together.

## Setup

```bash
git clone --recurse-submodules https://github.com/amir734jj/stream-subscription.git
cd stream-subscription
cp .env.example .env
# Edit .env with your values
```

## Configuration

| Variable | Description | Default |
|---|---|---|
| `DATABASE_URL` | PostgreSQL connection string for the API | — |
| `UI_PORT` | Host port for the UI | `8080` |

## Run

```bash
docker compose up -d
```

## Submodules

- `api/` — [stream-subscription-api](https://github.com/amir734jj/stream-subscription-api)
- `ui/` — [stream-subscription-ui](https://github.com/amir734jj/stream-subscription-ui)

To update submodules:

```bash
git submodule update --remote
```
