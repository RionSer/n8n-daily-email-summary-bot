# Daily Email Summary Bot (n8n)

## Overview

This project is an automated daily news email workflow built using n8n. It retrieves the latest headlines from an RSS feed, selects the top stories, formats them into a structured HTML email, and sends them to a specified recipient every morning.

---

## How It Works

The workflow runs automatically every day at 08:00 and performs the following steps:

1. **Schedule Trigger**
   Initiates the workflow at a fixed daily time.

2. **Fetch RSS News**
   Retrieves the latest articles from the BBC News RSS feed:
   http://feeds.bbci.co.uk/news/rss.xml

3. **Limit Results**
   Selects the top five news items from the feed.

4. **Format HTML Email**
   Generates a clean HTML email that includes:

   * Current date
   * Article titles
   * Short descriptions
   * Links to full articles

5. **Send Email**
   Sends the formatted email using a configured Gmail account.

---

## Example Output

The recipient receives a structured email containing:

* A daily news header
* The current date
* Five curated news articles
* Direct links to read more

---

## Requirements

* n8n (cloud or self-hosted)
* Gmail account with OAuth2 credentials configured
* Internet access to RSS feeds

---

## Setup Instructions

1. Import the provided JSON workflow into n8n.
2. Configure Gmail OAuth2 credentials.
3. Update the recipient email address.
4. Activate the workflow.

---

## Features

* Automated daily execution
* Structured and readable email format
* Simple and extensible workflow design
* Easy integration with other services

---

## Customization

This workflow can be extended in several ways:

* Replace the RSS source with a different feed (technology, finance, sports, etc.)
* Add multiple RSS sources
* Filter articles by keywords or categories
* Send emails to multiple recipients
* Integrate with messaging platforms such as Slack or Telegram
* Add AI-based summarization of articles

---

## Use Cases

* Personal daily news briefing
* Team or company updates
* Industry-specific newsletters
* Automated content aggregation

---

## Notes

* Ensure Gmail API usage limits are respected
* RSS feed availability depends on the provider
* Keep credentials secure within n8n

---


## Built With

* n8n
* Gmail API
* RSS feeds



