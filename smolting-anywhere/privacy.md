---
title: Smolting Anywhere — Privacy Policy
---

# Smolting Anywhere — Privacy Policy

_Last updated: 2026-11-02_

Smolting Anywhere is a browser extension (Chrome, Edge and other Chromium browsers) that draws
Smolting, a 3D ragdoll, on top of the page you are looking at. It is a toy. It does not collect,
store, transmit or sell any data about you or the pages you visit.

## What the extension does **not** do

- It does not read, record or transmit page content, URLs, browsing history, form input,
  cookies or anything else from the websites you use it on.
- It does not use analytics, telemetry, crash reporting, advertising or tracking of any kind.
- It does not run on any page until you click its toolbar button for that tab, and it stops
  again when you navigate away or turn it off.
- It does not have accounts, logins or a backend that knows who you are.

## What the extension **does**

- **Downloads the 3D model.** The first time Smolting appears, the extension fetches the
  Smolting model files (about 8 MB) from our content delivery network at
  `https://d344nqw9y6muw5.cloudfront.net/`. This is an ordinary HTTPS download, like loading
  an image; the request carries no identifying information from the extension (no IDs, no
  page URL). Like any web server, the CDN may log the requesting IP address and time for
  operational purposes. The files are then cached by the browser so later runs load from disk.
- **Receives Smolting's latest post.** While Smolting is on a tab (and the "Posts" setting is
  on), the extension keeps a one-way connection to our relay server
  (`https://smolting-feed-production.up.railway.app/`, hosted on Railway) which sends it the
  newest public post from the X account @inversebrah so it can be shown in a speech bubble.
  The request carries nothing from you or the page — no IDs, no URL, no cookies; like any web
  server, the relay may log the connecting IP address and time for operational purposes. The
  post's images and avatar load directly from X's image servers (`pbs.twimg.com`), inside the
  extension's own frame — the website you are on is not involved. Clicking the bubble opens that
  post on x.com in a new tab; nothing happens unless you click. Turn it off under Settings → Posts.
- **Stores your settings.** Toolbar edge, Smolting's size, the sound switch and the Posts switch
  are saved with the browser's extension sync storage (`chrome.storage.sync`) so they follow you
  to the browsers you are signed into. The id of the last post shown is kept in local extension
  storage so the same post is not announced twice. That storage holds nothing else and is
  removed when you uninstall the extension.
- **Remembers whether Smolting is on for a tab**, in memory only, for as long as the tab lives.

## Permissions

| Permission | Why |
| --- | --- |
| `activeTab` | Lets the extension act on the current tab only after you click its toolbar button. No access to other tabs or to sites in the background. |
| `scripting` | Injects the overlay into that tab when you click. |
| `storage` | Saves the settings above and the id of the last post shown. |

The extension requests no host permissions and declares no content scripts, so it cannot see
any page you have not explicitly turned it on for.

## Limited Use

The extension handles no user data, so there is nothing to transfer, sell or use for
advertising. Should that ever change, use of any data obtained through the extension will be
limited to providing and improving the features described in its store listing, in compliance
with the Chrome Web Store User Data Policy, including its Limited Use requirements.

## Children

The extension collects no data from anyone, including children.

## Changes and contact

If this policy ever changes, the new version is published here and the date at the top is
bumped. Questions: open an issue at
[github.com/Ritorai/smolting-policies](https://github.com/Ritorai/smolting-policies/issues).
