# webhoser

![webhose.io](http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/webhose-io-logo.png)

## Function

* `wh_token` - setup token
* `wh_news_filter` - Get news
* `wh_paginate` - paginate
* `wh_frame` - parse results

## Examples

``` r
token <- <- wh_token("xXX-x0X0xX0X-00X") # setup token

# get three pages on Barack Obama
token %>%  
  wh_news_filter(q = "World Economic Forum") %>% # basic example
  wh_paginate(p = 3) -> wef
```
