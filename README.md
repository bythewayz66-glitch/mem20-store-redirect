# mem20-store-redirect

Redirect layer for **mem20.store** and **www.mem20.store** → https://mem20.com

GitHub Pages allows exactly one custom domain per repository, so the alternate
hostnames each need their own tiny Pages site. This is the `mem20.store` one.

| File | Purpose |
|---|---|
| `CNAME` | `mem20.store` — this repo's single registered custom domain |
| `.nojekyll` | skip Jekyll; there is nothing to build |
| `index.html` | client-side redirect preserving path, query and hash |
| `404.html` | same redirect for any deep path that is not mirrored |

DNS it expects (already in place, do not change):

- `mem20.store`  A → 185.199.108.153 / .109.153 / .110.153 / .111.153
- `www.mem20.store` CNAME → `bythewayz66-glitch.github.io`
