---
title: Firefox Fixes
layout: default
---

### Preferences

- General
  - Play DRM-controlled content: ON
  - Firefox Updates: Check for updates but let you choose...
  - Recommend extensions as you browse: OFF
  - Recommend features as you browse: OFF
  - Network Settings:
    - Enable DNS over HTTPS: ON \\
      Provider: CloudFlare
- Home
  - Homepage: BLANK
  - New tabs: BLANK
  - Highlights: OFF
  - Snippets: OFF
- Search
  - Default Search Engine: DuckDuckGo
  - Provide search suggestions: OFF
- Privacy & Security
  - Content Blocking: STRICT
  - Permissions:
    - Block new requests asking to access...: (ALL) ON
  - Block pop-up windows: ON
  - Warn you when websites try to install add-ons: ON
  - Allow Firefox to install and run studies: OFF
  - Allow Firefox to make personalised extension recommendations: OFF
  - Allow Firefox to send backlogged crash reports...: OFF

### Must-Have Extensions

- [Multi-Account Containers](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/)
- [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/)
- [Redirector](https://addons.mozilla.org/en-GB/firefox/addon/redirector/)
- [Merge Windows](https://addons.mozilla.org/en-US/firefox/addon/merge-window/)

### Cool Extensions

- [Gesturefy](https://addons.mozilla.org/en-US/firefox/addon/gesturefy/)
- [Laser Cat](https://addons.mozilla.org/en-US/firefox/addon/the-laser-cat/)
- [Dark Mode](https://addons.mozilla.org/en-US/firefox/addon/dark-mode-webextension/)

### userChrome

I've gone a bit further and customised the CSS of the browser itself
with a [userChrome](https://www.userchrome.org/) file:

- [my userChrome.css](/etc/userChrome.css)
