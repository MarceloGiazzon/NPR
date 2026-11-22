# NPR — NPDev Pack Repo

A catalog of reusable [NPDev](https://github.com/MarceloGiazzon/NPDevGeneral) packs, fetchable via
`npdev pack add` using the `git+https` coordinate grammar:

```
git+https://github.com/MarceloGiazzon/NPR.git//packs/<name>@<tag>
```

Each pack lives in its own directory under `packs/`, one `pack.json` per pack, tagged at each
published version.

## Packs

- **[user](packs/user/pack.json)** (`v1.0.0`) — a portable credential bond for an `identity::User`:
  a password hash tied 1:1 to an identity user. Depends on the `identity` pack.

## Pack catalog for AIs

12 reusable packs, described in two small levels so an AI can pick one without reading it.

1. **Index** - one line per pack (`id|kind|area|trust|need|requires:...`, trust is `draft`, `verified` or `certified`):
   https://raw.githubusercontent.com/MarceloGiazzon/NPR/main/catalog/l0.txt
2. **Card** - about 300 tokens per pack: concepts with key fields and states, roles to bind, flows, events, screens, the exact `packs[]` line to consume it, and its main limit:
   https://raw.githubusercontent.com/MarceloGiazzon/NPR/main/catalog/cards/<id>.json  (for example https://raw.githubusercontent.com/MarceloGiazzon/NPR/main/catalog/cards/helpdesk.json)

Read the index, pick the packs that match the need, read only their cards, then put the `use` line of each card in the model's `packs[]`. Prefer a catalog pack to re-modelling what it already covers.
