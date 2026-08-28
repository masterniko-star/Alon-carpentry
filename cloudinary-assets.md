# Cloudinary assets

Cloud name: `zrevzjvb`
Folder: `nagar-alon-pics`
Uploaded: 2026-08-27

Base URL: `https://res.cloudinary.com/zrevzjvb/image/upload/`

| Local file | public_id | Size (px) | URL |
|---|---|---|---|
| pics/logo1.png | nagar-alon-pics/logo1 | 1672x941 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/logo1.png |
| pics/logo2.png | nagar-alon-pics/logo2 | 1254x1254 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/logo2.png |
| pics/logo3.png | nagar-alon-pics/logo3 | 1536x1024 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/logo3.png |
| pics/logo4.png | nagar-alon-pics/logo4 | 1774x887 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/logo4.png |
| pics/pic_alon (1).png | nagar-alon-pics/pic_alon_1 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_1.png |
| pics/pic_alon (2).png | nagar-alon-pics/pic_alon_2 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_2.png |
| pics/pic_alon (3).png | nagar-alon-pics/pic_alon_3 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_3.png |
| pics/pic_alon (4).png | nagar-alon-pics/pic_alon_4 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_4.png |
| pics/pic_alon (5).png | nagar-alon-pics/pic_alon_5 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_5.png |
| pics/pic_alon (6).png | nagar-alon-pics/pic_alon_6 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_6.png |
| pics/pic_alon (7).png | nagar-alon-pics/pic_alon_7 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_7.png |
| pics/pic_alon (8).png | nagar-alon-pics/pic_alon_8 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_8.png |
| pics/pic_alon (9).png | nagar-alon-pics/pic_alon_9 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_9.png |
| pics/pic_alon (10).png | nagar-alon-pics/pic_alon_10 | 1122x1402 | https://res.cloudinary.com/zrevzjvb/image/upload/nagar-alon-pics/pic_alon_10.png |

## Notes

- Spaces and parentheses in the original file names were normalized to
  underscores in the `public_id` (`pic_alon (1).png` -> `pic_alon_1`).
- Add transformations right after `/upload/`, e.g.
  `.../upload/f_avif,q_auto:eco,w_800/nagar-alon-pics/logo1.png`.

## Delivery convention

Content images are delivered through `<picture>` with two candidate formats:

| Purpose | Transformation prefix |
|---|---|
| `<source type="image/avif">` | `f_avif,q_auto:eco,…` |
| `<img>` fallback | `f_auto,q_auto:eco,…` |

`f_auto` is **not** enough on its own here: this account's auto-format serves
WebP, never AVIF, even when the browser advertises AVIF support. Measured on
`pic_alon_1` at `ar_4:5,w_800` — WebP `q_auto` 55.9 KB, WebP `q_auto:eco`
47.0 KB, AVIF `q_auto:eco` 25.4 KB.

srcset widths in use:

| Slot | Widths |
|---|---|
| Hero (`ar_3:2`) | 480, 560, 760, 1120 |
| Gallery tile (`ar_4:5`) | 400, 560, 720, 800 |
| About (`ar_4:5`) | 360, 560, 700 |
| Header logo | 272, 360, 540 |
| Footer logo | 264, 396 |

`og:image`, the schema.org logo and the favicon stay on plain `f_auto,q_auto` —
social scrapers and favicon fetchers are not always AVIF-capable, and `f_auto`
already falls back to JPEG/PNG for them.
