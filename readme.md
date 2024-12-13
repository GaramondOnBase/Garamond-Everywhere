# Garamond Everywhere

This Chrome extension replaces the font on all web pages with the beautiful **EB Garamond**. Bring style and history to the web, one page at a time!

This project is copypasta of [r4topunk](https://warpcast.com/r4topunk/0x1036d6cd)'s [code](https://github.com/r4topunk/comic-sans-everywhere). That project is a remix of [jtgi](https://warpcast.com/jtgi/0xdf3c8658)'s code.

## Features

- Applies the EB Garamond font to **all text** on every webpage.
- Lightweight and simple: just install and enjoy!
- Perfect for Garamond enthusiasts.

## Installation

1. Clone this repository:

```bash
git clone https://github.com/garamondonbase/garamond-everywhere.git
cd garamond-everywhere
```

2. Open Chrome and navigate to chrome://extensions/.
3. Enable Developer Mode (toggle in the top-right corner).
4. Click Load unpacked and select the folder where this repository is cloned.
5. Refresh any open tabs, and EB Garamond will take over the web!

## Files in the Repository

• manifest.json: Defines the metadata and behavior of the extension.
• content.js: Contains the script to inject the EB Garamond font into every webpage.

## Example Code

The key part of the extension is the code in content.js:

```js
const styleElement = document.createElement("style");
styleElement.innerHTML = '* { font-family: "EB Garamond" !important; }';
document.head.appendChild(styleElement);
```
