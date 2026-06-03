# Day 35: Mini Project – Autonomous Research Assistant

## Learning Goals
- Build an agent that can search the web, read web pages, and synthesise a structured report.
- Combine tools: web search, URL scraping, text summarisation.
- Produce a final research report with citations.

## Project Overview
The agent takes a research question (e.g., “Latest advances in quantum computing”), searches for relevant articles, extracts content, summarises each, and compiles a final answer.

## Topics Covered
1. Web search via Tavily or SerpAPI.
2. Fetching and cleaning web page text.
3. Summarising long web content using map‑reduce.
4. Final report generation with citations.

## Setup
```bash
pip install langchain langchain-openai tavily-python beautifulsoup4 requests