# 📘 Facebook Scraper API — Documentation

> Unlock Facebook data effortlessly with powerful scraping tools. Extract page names, URLs, contact info, likes, followers, posts, comments, Marketplace listings, and Meta Ads metrics.

[![RapidAPI](https://img.shields.io/badge/RapidAPI-Subscribe-blue?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAAC1SURBVChTY/hPADCgC2zatOk/kPkfxgYBkBiKRjBgYmL6D1IBooFsFBcjA5AmEI0OQGxkNYQBSBMhNVCN/0E0XhqZmJj+gzQiC8I0EaURpglZI0gTSBxZIz6NME3oGnFpxKUJphGXRnyaYBqxacSnCaYRXSM+TegasTTi04SuEUsj2ZpgGrE04tOE0IhFIyFNQDYDSCOIjQ5AYhgA3d4gDCSD+ExMTDAaRIPkYXwGBgYAd3UrljKFVPIAAAAASUVORK5CYII=)](https://rapidapi.com/oussemaf/api/facebook-scraper-api4)
[![Endpoints](https://img.shields.io/badge/Endpoints-35-green?style=for-the-badge)]()
[![Version](https://img.shields.io/badge/Version-v1-orange?style=for-the-badge)]()
[![Live Docs](https://img.shields.io/badge/Live_Docs-Swagger_UI-85EA2D?style=for-the-badge&logo=swagger)](https://minima-partners.github.io/facebook-scraper-api-docs/)
[![Postman](https://img.shields.io/badge/Postman-Docs-FF6C37?style=for-the-badge&logo=postman)](https://documenter.getpostman.com/view/7191741/2sBXigMZ5Y)

---

## 📂 What's in this repo

| File | What it does |
|------|-------------|
| [`index.html`](./index.html) | **Interactive Swagger UI docs** — enable GitHub Pages and share the link |
| [`facebook_scraper_api_openapi.yaml`](./facebook_scraper_api_openapi.yaml) | **OpenAPI 3.0 Spec** — import into Swagger Editor, Redocly, Stoplight, etc. |
| [`facebook_scraper_api_postman.json`](./facebook_scraper_api_postman.json) | **Postman Collection v2.1** — import into Postman and start testing |
| [`README.md`](./README.md) | This documentation |

---

## 🚀 Quick Start

### Import into Postman (recommended)
1. Open **Postman** → click **Import** → upload `facebook_scraper_api_postman.json`
2. Go to **Collection Variables** and set `rapidapi_key` to your RapidAPI key
3. All 35 endpoints are ready — pick one, hit **Send**

### Browse Interactive Docs
Visit the **live Swagger UI** page:
> `https://minima-partners.github.io/facebook-scraper-api-docs/`

*(Replace `YOUR_USERNAME` with your GitHub username after enabling GitHub Pages)*

### Use the OpenAPI Spec
Import `facebook_scraper_api_openapi.yaml` into:
- [Swagger Editor](https://editor.swagger.io)
- [Redocly](https://redocly.com)
- [Stoplight](https://stoplight.io)
- Any OpenAPI 3.0 compatible tool

---

## 🔐 Authentication

All requests require these headers:

| Header | Value |
|--------|-------|
| `x-rapidapi-key` | Your RapidAPI subscription key |
| `x-rapidapi-host` | `facebook-scraper-api4.p.rapidapi.com` |

**Base URL:** `https://facebook-scraper-api4.p.rapidapi.com`

Get your API key by subscribing at [RapidAPI](https://rapidapi.com/oussemaf/api/facebook-scraper-api4).

---

## 📋 All 35 Endpoints

### Facebook Pages Details/Posts
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/get_facebook_page_id` | Get the unique ID of any Facebook Page |
| `GET` | `/get_facebook_pages_details_from_link` | Extract essential page data (bio, email, followers, rating, etc.) |
| `GET` | `/get_facebook_page_posts_details_from_id` | Get latest page posts (up to 3 per request) |
| `GET` | `/get_facebook_page_videos_details` | Get page videos (up to 6 per request) |
| `GET` | `/get_facebook_reels_details` | Get page reels (up to 10 per request) |

### Facebook Groups Details/Posts
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/get_facebook_group_id` | Get the unique ID of any Facebook Group |
| `GET` | `/get_facebook_group_metadata_details` | Get group metadata (name, id, url, image) |
| `GET` | `/get_facebook_group_details_from_id` | Full group details (members, rules, activity) |
| `GET` | `/get_facebook_group_posts_details_from_id` | Get latest group posts (up to 3 per request) |
| `GET` | `/get_facebook_group_videos_details_from_id` | Get group videos (up to 6 per request) |

### Facebook Posts Details
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/get_facebook_post_id` | Extract post ID from a Facebook URL |
| `GET` | `/get_facebook_post_details` | Get full post details |
| `GET` | `/get_facebook_post_comments_details` | Get post comments (up to 10 per request) |
| `GET` | `/get_facebook_post_comment_replies` | Get replies to a specific comment |
| `GET` | `/get_facebook_post_attachement_details` | Get post attachments and reactions |
| `GET` | `/get_facebook_video_post_details` | Get video post details |

### Facebook Search
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/fetch_search_pages` | Search Facebook pages |
| `GET` | `/fetch_search_people` | Search Facebook people |
| `GET` | `/fetch_search_locations` | Search Facebook locations |
| `GET` | `/fetch_search_posts` | Search Facebook posts |
| `GET` | `/search_facebook_watch_videos` | Search Facebook Watch videos |

### Meta Ads Library Search
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/get_supported_countries` | List all supported country codes |
| `GET` | `/fetch_search_ads_pages` | Search ad pages (GET method) |
| `POST` | `/fetch_search_ads_pages` | Search ad pages (POST, for long cursors) |
| `GET` | `/fetch_page_ad_details` | Get page ad details |
| `GET` | `/fetch_archive_ad_details` | Get archived ad details |
| `GET` | `/fetch_search_ads_keywords` | Search ads by keyword |

### Facebook Marketplace Listings
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/get_facebook_marketplace_items_listing` | Search marketplace items with advanced filters |
| `GET` | `/get_listing_item_details` | Get specific listing details |
| `GET` | `/get_seller_details` | Get seller profile, ratings, reviews |
| `GET` | `/get_marketplace_categories` | List all marketplace categories |
| `GET` | `/find_city_coordinates` | Get city coordinates for location filters |
| `GET` | `/facebook_marketplace_vehicles_listings` | Search vehicle listings |
| `GET` | `/facebook_marketplace_rentals_listings` | Search rental property listings |

### Facebook Download Media
| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/download_media` | Download media (images, videos, audio) from Facebook URLs |

---

## 📄 Pagination

Most list endpoints support cursor-based pagination. The response includes:

```json
{
  "page_info": {
    "end_cursor": "abc123...",
    "has_next": true
  }
}
```

Pass `end_cursor` as a query parameter in the next request to fetch more results.

---

## 🔗 Links

- **Subscribe:** [RapidAPI - Facebook Scraper API](https://rapidapi.com/oussemaf/api/facebook-scraper-api4)
- **Postman Docs:** [documenter.getpostman.com](https://documenter.getpostman.com/view/7191741/2sBXigMZ5Y)
- **Swagger UI:** [minima-partners.github.io](https://minima-partners.github.io/facebook-scraper-api-docs/)
- **Pricing:** Freemium (free tier available)

---

## ⚙️ Enable GitHub Pages (for live Swagger UI)

1. Go to your repo **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / root
4. Save — your docs will be live at `https://minima-partners.github.io/facebook-scraper-api-docs/`

---

*Last updated: March 2026*
