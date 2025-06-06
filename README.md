# 📌 Project: Scraping Top Repositories for Topics on GitHub

## TODO (Intro)

### 🔎 Introduction about Web Scraping

Web scraping is an automated method used to extract large amounts of data from websites quickly and efficiently. It enables us to gather structured information from dynamic websites that do not offer easy APIs or data dumps.

### 🌐 Introduction about GitHub and the Problem Statement

GitHub is the world’s leading platform for hosting and collaborating on code. It hosts millions of repositories across a wide range of topics and domains. However, GitHub does not provide an easy way to **export** or **list** the top repositories within a topic, making it challenging for researchers, data scientists, or developers to analyze and discover relevant projects at scale.  
In this project, we will scrape GitHub’s Topics page to identify the top repositories for each topic and store them in structured CSV files.

### 🛠️ Tools Used

We will use the following tools:

- **Python**: Our main programming language for scripting and data processing.
- **requests**: A popular Python library for sending HTTP requests to fetch HTML content.
- **BeautifulSoup**: A powerful HTML parser for extracting data from web pages.
- **pandas**: A data manipulation library to clean and store the scraped data in CSV files.

---

### 📝 Steps We’ll Follow

1. Scrape the [GitHub Topics page](https://github.com/topics).
2. Extract the following information for each topic:
   - **Topic Title**  
   - **Topic Page URL**  
   - **Topic Description**
3. For each topic, navigate to its page and extract the top 25 repositories, including:
   - **Repo Name**  
   - **Username**  
   - **Stars**  
   - **Repo URL**
4. Create a **CSV file** for each topic in the following format:

```csv
Repo Name,Username,Stars,Repo URL
three.js,mrdoob,69700,https://github.com/mrdoob/three.js
libgdx,libgdx,18300,https://github.com/libgdx/libgdx
