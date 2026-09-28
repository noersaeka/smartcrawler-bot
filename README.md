# SmartCrawler

SmartCrawler is a small, experimental crawler that collects publicly listed
product information (name, price, size, availability) from online shops for
price-comparison research.

**How it behaves**
- It follows robots.txt for the user-agent `SmartCrawler`.
- It sends about one request per second per site, and backs off when asked
  (HTTP 429 / Retry-After).
- It does not log in, bypass bot checks, or collect personal data.
- It currently visits a small number of sites, roughly every two days.

**To stop it visiting your site**, add this to your robots.txt:

    User-agent: SmartCrawler
    Disallow: /

or email: ventlasiete@gmail.com
