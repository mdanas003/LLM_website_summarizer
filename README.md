# LLM_website_summarizer
An AI-powered tool that extracts the content of a webpage and generates a concise summary using a Large Language Model (LLM).

This project demonstrates how web scraping and LLM APIs can be combined to automatically summarize web pages.

---

## Features

* Scrapes webpage content using BeautifulSoup
* Cleans and extracts relevant text from HTML
* Uses an LLM to generate a short summary
* Supports Markdown output formatting
* Uses environment variables to securely store API keys

---

## Tech Stack

* Python
* OpenAI API
* BeautifulSoup
* Requests
* python-dotenv

---

## Project Workflow

URL → Web Scraper → Clean Text → Prompt Builder → LLM → Summary Output

1. The program downloads a webpage.
2. HTML is parsed and cleaned to remove scripts, styles, and images.
3. The relevant text content is extracted.
4. A structured prompt is sent to an LLM.
5. The LLM generates a concise summary of the webpage.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/llm-website-summarizer.git
cd llm-website-summarizer
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Environment Setup

Create a `.env` file:

```
OPENAI_API_KEY=your_api_key_here
```

---

## Usage

Run the summarizer and provide a URL:

```python
display_summary("https://example.com")
```

The program will fetch the webpage and generate a summary using the LLM.

---

## Example

Input:

```
https://www.w3schools.com/python/python_comments.asp
```

Output:

A concise AI-generated summary of the webpage.

---

## Future Improvements

* Multi-page website summarization
* Link extraction and relevance filtering
* Support for local models using Ollama
* CLI interface for easier usage
* Streamed responses from the LLM

---

## Author

Mohammed Anas
B.Tech IT Student | AI & ML Enthusiast
