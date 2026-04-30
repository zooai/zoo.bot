# zoo.bot landing site

Static landing page for the Zoo Bot project (the agent runtime forked from
hanzo.bot at `~/work/zoo/bot`).

This repo only contains the marketing site. The actual CLI/runtime lives at
`~/work/zoo/bot` (GitHub: `zooai/bot`).

## Deploy

Deployed to Cloudflare Pages project `zoo-bot`, custom domains `zoo.bot` and
`www.zoo.bot`. CF zone id: `69cbabebead4a6f9d17c46db3d746d9a`.

```sh
wrangler pages deploy public --project-name zoo-bot --branch main
```

## DNS

Both apex and www are CNAME → `zoo-bot.pages.dev`, proxied through CF.
Zone activates once registrar (Porkbun) NS is updated to:
- `aron.ns.cloudflare.com`
- `clay.ns.cloudflare.com`

## Brand

- Color: `#00cc66` (zoo green)
- Logo: `public/zoo-logo.svg`
- Foundation: Zoo Labs Foundation, 501(c)(3)
- Twitter: `@zoo_labs`
- GitHub org: `zooai`
