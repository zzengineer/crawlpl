# crawlpl
compact crawling tools written in perl

---
### NAME
rexcrawl -- crawler with regex patterns for content and crawl-urls

csscrawl -- crawler with css selector patterns for content and crwal-urls (broken) 

mixcrawl -- crawler with css selector patterns for content and regex for crawl-urls

### SYNOPSIS

`rexcrawl url extract-pattern [crawl-pattern]`

`csscrawl url extract-selector [crawl-selector]`

`mixcrawl url extract-selector [crawl-pattern]`

### DESCRIPTION

to be continued

### EXAMPLES

```
* crawl searchresult headers
rexcrawl http://www.google.com/search?q=test  '<h3.*<\/h3>'

* crawl searchresult headers and descend to subpages
rexcrawl http://www.google.com/search?q=test  '<h3.*<\/h3>'  'http:\/\/.*start[^"]+'

csscrawl ---

* crawl searchresult headers
mixcrawl http://www.google.com/search?q=test  'h3.r'

* crawl searchresult headers and descend to subpages
mixcrawl http://www.google.com/search?q=test  'h3.r'  'http:\/\/.*start[^"]+'
```
