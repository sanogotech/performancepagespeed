# Performance :  Page Speed


##  Urls
- https://developers.google.com/speed/pagespeed/insights/
- https://github.com/GoogleChrome/lighthouse/blob/d2ec9ffbb21de9ad1a0f86ed24575eda32c796f0/docs/scoring.md#how-are-the-scores-weighted

- https://chrome.google.com/webstore/detail/performance-scorecard/aefnmfmlbjcdihkegonofhkijbdkcpoc
- DevTools Chrome Performance

## Lighthouse

There were issues affecting this run of Lighthouse:
Chrome extensions negatively affected this page's load performance. Try auditing the page in incognito mode or from a Chrome profile without extensions.

##  Using the Node CLI
Installation:

npm install -g lighthouse

Examples:
  lighthouse <url> --view                                                   Opens the HTML report in a browser after the run completes
  lighthouse <url> --config-path=./myconfig.js                              Runs Lighthouse with your own configuration: custom audits, report
                                                                            generation, etc.
  lighthouse <url> --output=json --output-path=./report.json --save-assets  Save trace, devtoolslog, and named JSON report.
  lighthouse <url> --emulated-form-factor=none                              Disable device emulation and all throttling.
    --throttling-method=provided
  lighthouse <url> --chrome-flags="--window-size=412,660"                   Launch Chrome with a specific window size
  lighthouse <url> --quiet --chrome-flags="--headless"                      Launch Headless Chrome, turn off logging
  lighthouse <url> --extra-headers "{\"Cookie\":\"monster=blue\"}"          Stringify\'d JSON HTTP Header key/value pairs to send in requests
  lighthouse <url> --extra-headers=./path/to/file.json                      Path to JSON file of HTTP Header key/value pairs to send in requests
  lighthouse <url> --only-categories=performance,pwa                        Only run the specified categories. Available categories: accessibility,
                                                                            best-practices, performance, pwa, seo.

For more information on Lighthouse, see https://developers.google.com/web/tools/lighthouse/.
