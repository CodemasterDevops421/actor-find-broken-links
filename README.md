Here's your updated `README.md` file tailored to include your Apify actor links and streamlined to fit your specified structure:

```markdown
## What does Broken Links Checker do?
Our Broken Links Checker is an intuitive SEO tool designed to improve your website's UX and SEO score, enhance your ranking, and prevent link decay.

## How does it check for broken links?
Broken Link Checker performs the following tasks:
- Generates a detailed report identifying either all or only the broken links on a website.
- Scans single or multiple websites simultaneously.
- Checks both domains and subdomains.
- Identifies broken link fragments.
- Delivers a comprehensive report directly to your email upon completion of the SEO inspection.
- Allows both manual and scheduled checks through a robust scheduling system.

## How much does it cost to run Broken Links Checker?
The basic plan costs approximately **USD 1 in Apify platform credits per 1,000 scraped results**. For more pricing details, visit our [pricing page](https://apify.com/pricing/actors).

## How to start Broken Links Checker
To use Broken Links Checker, follow these steps:
1. Click on *Try for free*.
2. Enter one or more URLs to start the audit.
3. Enable the *Save only broken links* option.
4. Add your email address to receive the SEO report.
5. Click *Run* and await the results.
6. Optionally, schedule the tool to perform regular checks.

For detailed setup instructions, visit our [step-by-step guide](https://blog.apify.com/step-by-step-guide-to-using-broken-links-checker/).

## Under the Hood
The checker begins at a specified URL and crawls all linked pages. It inspects each page for functional links, checking if linked pages load correctly and if they contain specified fragments.

## Input Options
Configure the actor on the [Apify platform](https://console.apify.com/) with these inputs:
- **Website URL**: Starting point for the link check.
- **Max pages**: Limits the number of pages checked.
- **Notification emails**: Email to receive notifications.
- **Save only broken links**: Option to report only broken links.
- **Crawl subdomains**: Enables checking within subdomains.

### Input Example
```json
{
  "baseUrl": "https://blog.apify.com",
  "maxPages": 1000,
  "notificationEmails": ["your.email@apify.com"],
  "saveOnlyBrokenLinks": true,
  "crawlSubdomains": true
}
```

## Output
The output is stored in your key-value store in two formats:
- `OUTPUT.json`: A JSON report of the results.
- `OUTPUT.html`: An HTML report for easy reading.

### Output Example
```json
[
  {
    "url": "https://blog.apify.com",
    "title": "Apify Blog: Web scraping and automation stories",
    "links": [
      {
        "url": "https://apify.com/",
        "normalizedUrl": "https://apify.com",
        "httpStatus": 200,
        "fragment": "",
        "fragmentValid": true,
        "crawled": true
      },
      ...
    ]
  }
]
```

## Explore More Tools
Discover other SEO tools and resources at [Apify Store](https://apify.com/dainty_screw).
```

