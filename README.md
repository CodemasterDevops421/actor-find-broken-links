
```markdown
# Broken Links Checker

## Overview
Our Broken Links Checker is a sophisticated SEO tool designed to enhance your website's user experience (UX) and search engine optimization (SEO) score. It helps improve your ranking and prevent link decay by identifying and reporting broken links.

## Features
- **Comprehensive Reporting**: Generates detailed reports highlighting both broken and functional links.
- **Multi-Website Capability**: Capable of scanning single or multiple websites simultaneously.
- **Domain and Subdomain Checks**: Efficiently checks both domains and subdomains for broken link fragments.
- **Email Reporting**: Sends comprehensive reports directly to your email upon completion.
- **Flexible Scheduling**: Supports both manual and scheduled checks.

## Cost Details
Running the Broken Links Checker costs approximately **USD 1 in Apify platform credits per 1,000 scraped results**. For additional pricing details, please visit our [pricing page](https://apify.com/pricing/actors).

## Getting Started
Follow these steps to start using the Broken Links Checker:
1. **Sign Up**: Click on *Try for free* on the Apify platform.
2. **Input URLs**: Enter one or more URLs to begin the audit.
3. **Set Preferences**: Enable the *Save only broken links* option.
4. **Receive Reports**: Add your email address to receive the SEO report.
5. **Start the Check**: Click *Run* and wait for the results.
6. **Schedule Checks**: Optionally, set up the tool to perform regular checks.

For a detailed setup guide, refer to our [step-by-step tutorial](https://blog.apify.com/step-by-step-guide-to-using-broken-links-checker/).

## How It Works
Starting from a given URL, the checker crawls all linked pages within the site, inspecting each for functional integrity and verifying that linked pages load correctly and contain specified fragments.

## Configuration
Set up the Broken Links Checker with the following inputs:
- **Website URL**: The starting URL for the link check.
- **Max pages**: Limits the scope of the check.
- **Notification emails**: Specifies the recipient of completion alerts.
- **Save only broken links**: Toggles between saving all links or only broken ones.
- **Crawl subdomains**: Enables the inspection of subdomains.

### Example Input
```json
{
  "baseUrl": "https://blog.apify.com",
  "maxPages": 1000,
  "notificationEmails": ["your.email@apify.com"],
  "saveOnlyBrokenLinks": true,
  "crawlSubdomains": true
}
```

## Output Details
Results are stored in two formats in your key-value store:
- `OUTPUT.json`: JSON formatted report of the findings.
- `OUTPUT.html`: HTML formatted report for easy review.

### Example Output
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
      }
    ]
  }
]
```

## Connect With Us

- **YouTube**: [Visit our channel](https://www.youtube.com/channel/UCSglWXooehH8Cy7LYHhXtqA)
- **Instagram**: [Follow us on Instagram](https://www.instagram.com/quicklifesolutionsofficial/)
- **AI Newsletter**: [Subscribe to our newsletter](https://sendfox.com/quicklifesolutions)
- **Free Consultation**: [Book a free consultation call](https://tidycal.com/quicklifesolutions/free-consultation)
- **More Tools**: [Explore our Apify actors](https://apify.com/dainty_screw)

### Support

- **Discord**: [Raise a Support ticket here](https://discord.gg/2WGj2PDmHb)
- **Email**: [Contact us](mailto:codemasterdevops@gmail.com)

Explore additional SEO tools in the [Apify Store](https://apify.com/store).
```
