This is a scraper that runs on [Morph](https://morph.io). To get started [see the documentation](https://morph.io/documentation)

Add any issues to https://github.com/planningalerts-scrapers/issues/issues

## To run the scraper

```
bundle exec ruby scraper.rb
```

Set `MORPH_AUSTRALIAN_PROXY` to the url for an Australian proxy

### Expected output

```
Fetching public notices list from: https://onlineservice.launceston.tas.gov.au/eProperty/P1/PublicNotices/PublicNoticeDetails.aspx?r=P1.LCC.WEBGUEST&f=%24P1.ESB.PUBNOTAL.ENQ
Found 30 public notices
Skipping existing record: DA0004/2025
Skipping existing record: DA0301/2025
(etc)
Scraping Public Notice - Application Details for DA0405/2025
Saved record for DA0405/2025
Scraping Public Notice - Application Details for DA0412/2025
Saved record for DA0412/2025
Saved record for DA0540/2025
Scraping complete
```

Execution time ~ 43 seconds.

## To run style and coding checks

```
bundle exec rubocop
```

## To check for security updates

```
gem install bundler-audit
bundle-audit
```
