# 📊 Fetching & Converting API Data to CSV

This project demonstrates how to fetch JSON data from a public API, convert it into a pandas DataFrame, and save it as a clean CSV file for further use.

---

## 🔑 Steps I Followed

1. **Created an API Key**  
   - I signed up at [NewsAPI.org](https://newsapi.org/) and generated my free API key.  
   - If you want to try with a different dataset, you can also use:  
     - 🎬 [TMDB API (Movies Dataset)](https://developer.themoviedb.org/reference/intro/getting-started)  
     - 🌎 [RapidAPI Hub](https://rapidapi.com/hub) (for various free APIs)

2. **Explored the JSON Response**  
   - I used an online [JSON Viewer](https://jsonviewer.stack.hu/) to visualize and understand the structure of the API response.

3. **Fetched Data Using Python**  
   Example snippet:

   ```python
   import pandas as pd
   import requests

   # API endpoint (replace with your key)
   url = "https://newsapi.org/v2/everything?q=tesla&from=2025-08-18&sortBy=publishedAt&apiKey=YOUR_API_KEY"

   response = requests.get(url)
   data = response.json()

   # Extract only the articles
   articles = data.get("articles", [])

   # Convert to DataFrame
   df = pd.DataFrame(articles)

   # Save to CSV without index
   df.to_csv("news_articles.csv", index=False)
   print("Data saved to news_articles.csv")
