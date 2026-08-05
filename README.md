# EverEffect Briefs (PUBLIC)

**This repository is public and served by GitHub Pages.** Anything committed here is readable by
anyone who has the URL. Treat every file as if it were emailed to the client, because effectively
it has been.

## What may go in here

Only **client-safe** documents. A document is client-safe when all of the following are true:

1. It contains no internal pricing, rate card lines, or retainer figures.
2. It contains no read on the client that they did not volunteer themselves.
3. It contains no finding about the client that we have not yet told them.
4. It names no EverEffect colleague and no internal process decision.
5. It has passed the leak scan below with zero hits.

**Internal research never goes here.** It lives in the private `evereffect-client-research`
repository. If you are unsure which a document is, it is internal.

## The leak scan

Before committing, open the file in a browser and run this against it. Zero hits required.

```js
['parked','parking','godaddy','rate card','$100 per page','$900','$300 per month','retainer',
 'commission','internal','do not send','budget authority','storage maintenance']
  .filter(s => document.body.innerText.toLowerCase().includes(s))
```

Extend the list per document with the keywords of whatever blocking finding that engagement has.

## Crawler policy

Every page carries `<meta name="robots" content="noindex, nofollow, noarchive, nosnippet">` and
`robots.txt` disallows everything. Pages are reachable by link, not by search. Adding a page
without the meta tag defeats this, so check it every time.

`index.html` deliberately lists nothing. Someone who finds the root learns only that documents are
shared by direct link.

## Live pages

| Document | URL |
|---|---|
| Ryan Nelson, pre-call brief | `/ryan-nelson/pre-call/` |
| Ryan Nelson, market findings | `/ryan-nelson/findings/` |
