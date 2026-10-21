# Eduarte Horizontal Scroll Fix

This Chrome extension adds a horizontal scrollbar to Eduarte pages where log-form buttons, such as **Edit** or **Submit**, extend beyond the screen.

## Use

1. Open an Eduarte tab.
2. Select the extension's toolbar button to open its menu.
3. Select **Turn on fix** or **Turn off fix**. The menu also contains the manual console code, a **Copy code** button, and an F12 tutorial.

The choice is kept for that tab while it remains open, including when the page reloads or navigates within Eduarte. Other tabs are unaffected, and the extension only runs on `eduarte.nl` pages.

After updating an installed copy, select the reload icon for the extension on `chrome://extensions`, then reload the Eduarte tab once.

## Install from the included folder

1. Open `chrome://extensions` in Chrome/edge/firefox/opera.
2. Enable **Developer mode**.
3. Select **Load unpacked**.
4. Choose the `eduarte-horizontal-scroll-fix` folder.

## Install from the ZIP

Chrome normally installs locally created extensions through **Load unpacked**. Extract `eduarte-horizontal-scroll-fix.zip` first, then follow the steps above. The ZIP is useful for moving or sharing the extension.

## CSS applied when enabled

```css
html, body { max-width:100% !important; overflow-x:auto !important; }
.content-wrapper, .js-scroll-wrapper, form, .tasks, .week-planning { max-width:100% !important; box-sizing:border-box !important; overflow-x:auto !important; }
button, input[type=submit], input[type=button] { flex-shrink:0; }
```
