# AI Website Analyzer

### Website Summarizer + AI Brochure Generator

An AI-powered tool that **analyzes a website, extracts important information, and generates structured summaries and company brochures using Large Language Models (LLMs).**

This project demonstrates how **web scraping, structured prompting, and LLM reasoning** can be combined to build multi-step AI workflows.

---

# Features

### Website Summarizer

* Scrapes webpage content
* Cleans HTML and extracts relevant text
* Generates a concise summary using an LLM

### AI Brochure Generator

* Extracts all links from a website
* Uses an LLM to identify **relevant pages** (About, Careers, etc.)
* Scrapes those pages
* Generates a **structured company brochure**

### Additional Features

* JSON structured outputs from the LLM
* Markdown formatted responses
* Streaming responses support
* Secure API key handling with `.env`

---

# Tech Stack

* **Python**
* **OpenAI API**
* **BeautifulSoup**
* **Requests**
* **python-dotenv**

---

# System Architecture

```
Website URL
     ↓
Web Scraper
     ↓
Extract Website Links
     ↓
LLM selects Relevant Links
     ↓
Scrape Relevant Pages
     ↓
Aggregate Content
     ↓
LLM Generates Summary / Brochure
```

This architecture demonstrates a **multi-step LLM pipeline**, where the model is used not only for text generation but also for **reasoning and decision-making**.

---

# Project Workflow

1. A website URL is provided.
2. The scraper downloads the HTML content.
3. HTML is cleaned by removing scripts, styles, images, and inputs.
4. All links from the webpage are extracted.
5. An LLM identifies which links are relevant.
6. Relevant pages are scraped and combined.
7. The LLM generates a summary or brochure.

---

# Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/ai-website-analyzer.git
cd ai-website-analyzer
```

---

# Environment Setup

Create a `.env` file in the project directory:

```
OPENAI_API_KEY=your_api_key_here
```

⚠️ Never upload your `.env` file to GitHub.

---

# Usage

### Generate Website Summary

```python
display_summary("https://example.com")
```

### Generate Company Brochure

```python
create_brochure("Company Name", "https://companywebsite.com")
```

### Stream Brochure Output

```python
stream_brochure("Company Name", "https://companywebsite.com")
```

---

# Example

### Input

```
https://huggingface.co
```

### Output

A structured AI-generated brochure describing:

* Company overview
* Products and services
* Culture and hiring
* Relevant company information

---

# Future Improvements

* Parallel page scraping for faster processing
* URL normalization for relative links
* Caching LLM responses
* Web UI for easier interaction
* Support for local models using **Ollama**
* Vector search for large websites

---

# Author

**Mohammed Anas**
B.Tech IT Student | AI & ML Enthusiast



