# Google Play Store Apps Analysis (2010–2018)

Mini exploratory data analysis (EDA) project using **pandas** on a dataset of ~62,700 Android apps from the Google Play Store.

The notebook explores app popularity, monetization strategies, genre performance, user ratings behavior, and realistic expectations for new app developers.

## Project Goals

- Understand which app categories historically attracted the most downloads and daily engagement
- Analyze monetization patterns (ads, in-app purchases, paid apps)
- Identify market leaders per category
- Estimate realistic daily install numbers for a newly released app
- Examine rating behavior, review-to-rating ratios, and weighted average scores

## Dataset

**Source**: Aggregated Google Play Store metadata (likely scraped ~2018–2019)  
**Rows**: ~62,694 apps  
**Time range**: Apps released between January 2010 – November 2018  
**Main columns used**:

- `app_id`, `title`
- `min_installs`, `reviews`, `ratings`, `ratings_per_day`
- `score` (average rating), star distribution (1–5 stars)
- `genre`, `genre_id`
- `price`, `offers_iap`, `ad_supported`
- `released` (release date)

## Key Findings (Highlights)

| Question                                      | Top Answer / Insight                                                                 |
|:----------------------------------------------|:-------------------------------------------------------------------------------------|
| Genres with highest avg ratings/day           | Strategy, Action, Racing, Arcade, Social                                             |
| Genres with lowest avg ratings/day            | Events, Medical, Business, Education, Food & Drink                                   |
| Clear market leader per genre                 | Subway Surfers (Arcade), WhatsApp (Communication), Clash of Clans (Strategy), etc.   |
| Realistic daily installs expectation (median) | ~13 installs/day (across all apps ever released)                                     |
| Most common monetization pattern              | Free + Ads (~38%), Free + Ads + IAP (~17%), Completely free (~33%)                  |
| Highest weighted-average rating genres        | Parenting, Education, Books & Reference                                              |
| Top reviewed apps (all-time)                  | Instagram, WhatsApp, Clash of Clans, Messenger, Clean Master                        |
| Most common release year                      | 2018 (≈20,861 apps in dataset)                                                       |
| Genres with strongest review ↔ rating correlation | Racing, Events, Simulation, Action (positive correlation)                        |

## Repository Contents

```text
├── Mini Project on pandas.ipynb     ← main analysis notebook
├── google-play-store.csv            ← dataset (~62k rows)
├── README.md                        ← this file
