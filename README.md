# Social Media Engagement Optimization

This project simulates how machine learning can be used to **re-rank social media posts** to improve overall engagement. Inspired by real-world feed ranking systems (e.g., Facebook, Instagram, TikTok), it showcases end-to-end data science skills — from feature engineering to A/B test simulation.

---

## Goal

Build a model that predicts whether a social media post will receive high engagement, and use that model to **reorder the user feed** in a way that maximizes overall engagement.

---

## Dataset

Simulated dataset with 100,000 posts containing:
- Post metadata: Type, Content, Timestamp
- Audience data: Age, Gender, Location, Interests
- Engagement metrics: Likes, Comments, Shares, Impressions, Reach
- Campaign & Influencer info

---

##  Key Steps

### 1. Data Cleaning & EDA
- Parsed timestamps, removed nulls
- Analyzed post timing, length, hashtags, links
- Explored engagement distributions

### 2. Feature Engineering
- Created new features:
  - Post hour & day of week
  - Is weekend, has hashtags/links
  - Post length
- Created binary engagement label for classification

### 3.  Modeling
- Trained classification models (Logistic Regression, XGBoost)
- Evaluated precision, recall, AUC
- Predicted engagement probability scores for each post

### 4.  Feed Ranking Simulation
- Simulated:
  - Baseline feed (chronological)
  - ML-ranked feed (predicted engagement score)
- Measured total Likes + Comments + Shares
- Compared total engagement across both feeds

---

##  Results

| Metric                  | Value     |
|-------------------------|-----------|
| Baseline Engagement     | 88,445    |
| ML-Ranked Engagement    | 88,445    |
| Uplift                  | **0.00%** |

Although the ML-ranked feed produced no measurable uplift, the project provided valuable insights into the **limits of the current feature set**.

---

##  Key Takeaway

> The features used (e.g., post timing, hashtags, length) did not provide strong enough signal to meaningfully predict high-engagement posts.

This reflects a real challenge in product data science — building effective engagement models requires **richer behavioral and content features**, which we outline below.

---

##  Next Steps (Optional Future Enhancements)

These are not required — but demonstrate how the project could be expanded. These are the steps I will be taking for my next iteration of this with more data availability

- **Text/NLP features** from post content
- **Visual features** (image type, quality, colors)
- **User history** (follower-post relationships, past engagement)
- **Temporal decay** — giving newer posts more weight
- **Live A/B testing** on real users

---

## Author

Ramandeep Brar
[LinkedIn]([https://linkedin.com/in/your-profile](https://www.linkedin.com/in/ramansandhu1704/)) | [Portfolio]([https://yourportfolio.com](https://www.datascienceportfol.io/ramanbrar))

