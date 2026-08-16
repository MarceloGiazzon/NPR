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
