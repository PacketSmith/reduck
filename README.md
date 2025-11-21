# Reduck

DuckDuckGo's bang redirects are too slow. Add the following URL as a custom search engine to your browser. Enables all of DuckDuckGo's bangs to work, but much faster. Custom default search engine "bang" via `dfb` paramater in URL. Defaults to using DuckDuckGO if not specified

```
https://reduck.page.dev?q=%s&dfb=ddg
```

## How is it that much faster?

DuckDuckGo does their redirects server side. Their DNS is...not always great. Result is that it often takes ages.

This is solved by doing all of the work client side. Once you've visited to https://reduck.pages.dev once, the JS is all cache'd and will never need to be downloaded again. Your device does the redirects, not the server.
