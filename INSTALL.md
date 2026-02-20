## [LibreNMS](https://www.librenms.org)

#### Install the Stylus extension

This theme is applied via the [Stylus](https://github.com/openstyles/stylus) browser extension:

- [Chrome / Edge / Brave](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
- [Firefox](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)

#### Activating the theme

1. Click [install directly with Stylus](https://raw.githubusercontent.com/dracula/librenms/main/dracula.user.css);
2. In the Stylus tab, replace `your-ip-or-domain.com` with your LibreNMS server address;
3. Save and reload your LibreNMS instance.

#### Configuration for multiple servers

If you manage multiple instances, you can target them explicitly or use a pattern.

**Specific servers** — list each URL prefix in the document rule:

```css
@-moz-document url-prefix("http://192.168.1.50"), url-prefix("https://nms.yourcompany.com") {
```

**Any LibreNMS instance** — match any URL containing the word "librenms":

```css
@-moz-document regexp("https?://.*librenms.*") {
```
