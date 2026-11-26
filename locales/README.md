# Wizzly Translations

Welcome! This folder contains the official localization files for **Wizzly** (`en.json` is the source of truth).

Anyone can contribute a new language or improve an existing translation without needing access to the main app source code.

## How to Contribute a New Language

1. Copy [`en.json`](./en.json) and rename the copy using its ISO 639-1 language code (e.g. `tr.json` for Turkish, `de.json` for German, `ja.json` for Japanese, or `pt-br.json` for Brazilian Portuguese).
2. Update the `_meta` block at the top of your new file:
   ```json
   "_meta": {
     "code": "tr",
     "name": "Turkish",
     "nativeName": "Türkçe",
     "localeTag": "tr-TR",
     "author": "Your Name or GitHub Handle"
   }
   ```
3. Translate all string values into natural, concise phrasing in your language.
   - **Do NOT translate JSON keys** (only translate the values on the right side).
   - **Keep `{placeholders}` intact** (for example `{name}`, `{count}`, `{n}`, `{err}`, `{clock}`, `{percent}`). You may reorder them if needed for natural grammar.
   - Keep button labels and status subtitles reasonably short so they fit neatly inside the Dock, Notch, and Settings UI.
4. For the `widgets` section:
   - `weekdaysFull`: 7 items starting with **Sunday** (`[Sunday, Monday, ..., Saturday]`).
   - `weekdaysShortMon`: 7 short labels starting with **Monday** (`[Mon, Tue, ..., Sun]`).
   - `weekdaysInitialSun`: 7 single-letter initials starting with **Sunday** (`[S, M, T, W, T, F, S]`).
   - `monthsFull` & `monthsUpper`: 12 month names starting with **January**.
   - `dateFormat`: Uses `{weekday}`, `{day}`, and `{month}` (e.g. `"{day} {month} {weekday}"`).

## Testing Your Translation Live in Wizzly

You can test your `.json` file directly inside the installed Wizzly app before submitting it:

1. Open **Wizzly Settings → Behavior & Taskbar → Interface Language** and click **Locales Folder** (or open `%AppData%\com.wizzly.app\locales\` in File Explorer), OR click **Import JSON...** directly.
2. Place your `<code >.json` file (e.g. `tr.json`) in that folder and click **Reload** (or restart Wizzly).
3. Select your language from the dropdown (or use **Auto** if your Windows display language matches) and inspect Settings, Dock, Notch, Launchpad, Spotlight, and Desktop Widgets.

Any missing keys automatically fall back to `en.json`, so incomplete drafts are still safe to test.
