# Seedream 4.5 API (seedream-4.5 / seedream4.5) — api guide with published pricing

> **default $0.026** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-8112e5)** · **[Get an API key](https://go.apimart.ai/k-1c074f)**

Everything here refers to **seedream-4.5** — also written **seedream4.5** or **seedream 4.5**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `default` | $0.026 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $2.6 |
| 1,000 | $26 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"seedream-4-5","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
