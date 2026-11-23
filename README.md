# Sassy on Tech — Micro.blog theme

A dark, magazine-style custom theme for [sassyontech.com](https://sassyontech.com), built on Micro.blog's Blank theme.

## Install

1. On Micro.blog: **Design → Edit Custom Themes → New Theme**. Name it, and paste this repo's URL as the **Clone URL**.
2. Back on **Design**: set the theme to **Blank**, set **Custom theme** to the new theme, then **Update Design**.

## Settings

All settings live in `layouts/partials/sassy-settings.html` (headline, about box, Mastodon link, email, featured category, posts per page). Edit it in Micro.blog's theme editor.

## How the homepage works

- **Hero:** the 3 newest posts in the `Featured` category (topped up with the newest posts if there are fewer than 3).
- **Fresh off the bench:** the next 3 newest posts.
- **Latest posts:** everything else, paginated, with the sidebar.
- Only posts **with a title** appear on the homepage. Short untitled posts still show in the archive, categories and feeds.
- Card images come from the post's first photo. Posts without one get a text-only card.

## Menu

Pages marked "Include in navigation" in Micro.blog appear in the header menu. Category pages can be added the same way with a page that redirects to `/categories/<name>/`.

## Files

```
layouts/
  _default/baseof.html     page skeleton
  _default/single.html     pages (About etc.)
  _default/list.html       category pages
  post/single.html         blog posts
  index.html               homepage
  list.archivehtml.html    /archive/
  partials/                head, header, footer, logo, card, sidebar, pagination, post-image, settings
static/css/sassy.css       all styles
```

Fonts load from [Bunny Fonts](https://fonts.bunny.net) (EU-hosted, no tracking): Yellowtail, Space Grotesk, Inter, JetBrains Mono.
