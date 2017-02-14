# intl? cldr?

* Globalize uses Cldr data
* Cldr is huge, use npm package, cherrypick what you need

---

* Intl is inside the browser
* ie11+, no safari
* Financial Times has a polyfill api (but it still is huge)
* FT customized example:
  `script src="https://cdn.polyfill.io/v2/polyfill.min.js?features=Intl.~locale.fr,Intl.~locale.pt"`

[i18n]
