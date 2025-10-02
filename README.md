# Backpack Review Analysis

This project analyzes backpack reviews from Amazon.ca (educational only) using **Python and Jupyter Notebook**.  
The goal is to understand **what features customers value most**, and to identify **top vs bottom-rated products** through data analysis and visualization.

---

## 🚀 Project Workflow

### 1. Web Scraping
- Used `requests` + `BeautifulSoup` to scrape Amazon.ca search results for **“backpack”**.  
- Extracted product **title, price, rating, number of reviews**.  
- Note: Amazon scraping is unstable and against ToS for production, this was done only for learning purposes.  

### 2. Data Cleaning
- Converted prices (`$34.99` → `34.99`)  
- Extracted ratings (`4.6 out of 5 stars` → `4.6`)  
- Parsed reviews (`(97.7K)` → `97700`)  
- Removed missing or duplicate entries  

### 3. Exploratory Data Analysis (EDA)
- **Distributions**: price, ratings, number of reviews  
- **Scatter plot**: price vs rating (bubble size = reviews)  
- **Histograms**: reviews (log scale) and ratings  

### 4. Insights from Ratings
- **Average price:** ~$48.72  
- **Average rating:** ~4.52 ★  
- **Median reviews:** ~847  
- **Cheapest backpack:** $13.99  
- **Most expensive backpack:** $219.95  

### 5. Top vs Bottom Products
- **Top-rated (≥100 reviews):**  
  Affordable, mid-priced ($30–$60), feature-rich (Laptop compartment, USB charging, Waterproof, Travel-friendly).  
  Examples: *Laptop Backpack for Women (4.8★, 2300 reviews)*, *Tomtoc Travel Backpack (4.7★)*.  

- **Lowest-rated (≥100 reviews):**  
  Ultra-cheap basics or overpriced niche bags.  
  Examples: *SUPACOOL Casual Backpack (4.2★, 5100 reviews)*, *Thule DSLR Camera Bag ($199, 4.2★)*.  

### 6. Keyword Analysis
- **Top-rated keywords:** *Laptop, Travel, Waterproof, USB, Lightweight, Work*  
- **Bottom-rated keywords:** *Casual, Classic, Packable, Military, Camera*  
- 👉 Customers reward **utility features**; penalize **generic/basic or overpriced niche** items.  

### 7. Visualization
- 📊 Histograms of ratings, reviews, and prices  
- 📈 Price vs Rating scatter (bubble = popularity)  
- ☁️ Word clouds for top vs bottom products  


---

### 🛠️ Tech Stack
- **Python** (pandas, numpy)  
- **BeautifulSoup4** for scraping  
- **Matplotlib / Seaborn** for visualization  
- **WordCloud** for text analysis  
- **Jupyter Notebook** for workflow  

---

### ⚡ Findings
1. Mid-priced ($30–$60) backpacks dominate satisfaction.  
2. Features that customers love → *Laptop storage, USB charging, Waterproof, Travel-ready*.  
3. Lowest ratings are found in ultra-cheap or overpriced niche bags.  
4. Amazon reviews are generally inflated (even bottom products ~4.2★).  
5. Best value = **affordable + functional + durable** backpacks.  



