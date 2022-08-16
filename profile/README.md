## DN42.Wiki

This is an static generated clearnet copy of https://wiki.dn42 (https://dn42.dev) which powered by [Cloudflare Pages](https://pages.cloudflare.com/).

## How it works

There's a [crontab job](https://github.com/dn42-wiki/scripts/blob/master/update-github-wiki) running periodically (currently every 12 min) to check and update [wiki](https://github.com/dn42-wiki/wiki) (copy of raw wiki repo) and [dn42-wiki-rendered](https://github.com/dn42-wiki/dn42-wiki-rendered) (repo for static generated site files.)
Then, there's a Cloudflare Pages job linked to [dn42-wiki-rendered](https://github.com/dn42-wiki/dn42-wiki-rendered), which automatically deploy generated files (located at [/dist](https://github.com/dn42-wiki/dn42-wiki-rendered/tree/master/dist) folder) to the site https://dn42.wiki
