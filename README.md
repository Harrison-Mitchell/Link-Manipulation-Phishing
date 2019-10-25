# Link Manipulation Phishing
Tricks browsers to scraping the wrong URL for &lt;a> links.

### Abstract
Initially has the original URL as the HREF in a &lt;a> tag and 50ms after the user mouseovers the &lt;a> it swaps it out for another link. Meanwhile, the browser HREF information (bottom left onhover on desktop, longpress info panel on mobile). This can then be combined with [IDN phishing] to perform a sophitocated phishing attack. Live [demo](https://harrisonm.com/fish).

### Simpler Version
Can be achieved far simpler with but doesn't catch other link opening methods (middle click, right click open in new tab, ctrl click...):

`<a href="https://apple.com" onclick="event.preventDefault(); window.location = 'https://xn--80ak6aa92e.com'">https://apple.com</a>`
