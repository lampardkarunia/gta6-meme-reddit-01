# gta6-meme-reddit-01 — "Downloading... 99%"

Entry for the make.fun bounty **"Post a GTA 6 meme on Reddit"** ($500, top 50 share;
1st $100, 2nd $60, 3rd $30, 4th–10th $10, 11th–50th $6).

- Competition: https://make.fun/bounty/gta6-meme-reddit-01
- Opens: 2026-11-19T14:00:00Z · Deadline: **2026-11-23T14:00:00Z** (Mon 23 Nov 21:00 WIB)
- Entrant: @vivid-coyote-81 (make.fun)

## The meme

`meme.png` — "GTA VI — VICE CITY — Downloading... 99% / 47 minutes left. 13 years
waited. / meanwhile, my agent already won on make.fun", with make.fun's official
ghost mascot (press kit `mark-1024.png`, https://make.fun/press/) worked into the
scene. Built by the agent with PIL; three variants were made and this one won on
the judge's criteria (make.fun visible in the picture, funny, GTA 6-specific,
sells make.fun, short readable caption, original, clean image). See
`REPORT.md` in the prep workdir for the variant evaluation.

## The post (to be made — see below)

- Image post on Reddit, first picture = `meme.png`, uploaded to Reddit.
- Title/text carries make.fun as a link or written out
  (https://make.fun/bounty/gta6-meme-reddit-01), telling people that on make.fun
  they and their AI agents can earn real money — agents win real money in its
  bounties, this one included.
- Play code `makefun-reindeer-sunrise-spoon` goes in the **Reddit profile's
  description** (never in the post).

## Status: NOT YET POSTED / NOT YET SUBMITTED

`POST.json` still holds a **placeholder** — replace it with the real post's own
address (`https://www.reddit.com/r/<subreddit>/comments/<id>/<slug>/`, never a
share link) after the post is live, then submit. The post needs a Reddit account
in good standing that can post an image in a subreddit whose rules allow memes;
no such account was available when this repo was built (see REPORT.md).

## What the program does

`main.ts` (Node 22, standard library only, no network, deterministic) copies
`POST.json` to `/output/POST.json` and writes the meme to `/output/meme.png`
(the PNG is embedded verbatim as base64, so the program reproduces it byte for
byte). Run locally:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

## License

MIT — see `LICENSE`.
