# Articles archive (migrated from WordPress)

The BRSCC articles were originally served by a WordPress install mounted at
`https://brscc.org/articles/` (behind the custom PHP main site). This directory
is a complete, self-contained static archive of that content.

## Layout

- `articles/index.html` — article listing
- `articles/YYYY/MM/DD/<id>/index.html` — each article, at its **original permalink**
- `articles/<slug>/index.html` — standalone pages (privacy-policy, youth-group)
- `articles/assets/style.css` — styling
- `articles/wp-content/uploads/…` — all images/video, mirrored from the original
- `articles/backup/*.json` — raw source of truth from the WordPress REST API

## Raw backup (source of truth)

- `posts.json` — all 6 posts (full rendered content, dates, categories) via `/wp-json/wp/v2/posts?_embed`
- `pages.json` — pages via `/wp-json/wp/v2/pages`
- `media.json` — media library manifest (31 items) via `/wp-json/wp/v2/media`

To re-render the static site from the raw JSON, re-run the converter used to
produce these pages (upload URLs are rewritten from
`https://brscc.org/articles/wp-content/uploads/` to root-absolute
`/articles/wp-content/uploads/`).

## Articles

| Date | Title | Permalink |
|------|-------|-----------|
| 2024-09-16 | 09-21 Health Insurance Program 公益讲座 | /articles/2024/09/16/25/ |
| 2024-09-15 | 2024 穿月时空 BRSCC 中秋庆祝活动 | /articles/2024/09/15/10/ |
| 2024-08-13 | BRSCC 2-Day Summer Camp | /articles/2024/08/13/58/ |
| 2024-07-20 | BRSCC Youth Group Summer Fair | /articles/2024/07/20/36/ |
| 2024-02-04 | BRSCC 2024 半岛华人社区春晚视频 4K | /articles/2024/02/04/32/ |
| 2019-03-18 | Now we have our website | /articles/2019/03/18/1/ |

Archived on 2026-07-26.
