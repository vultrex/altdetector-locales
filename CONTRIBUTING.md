## 🌍 Translating Alt Detector

Thank you for your interest in translating **Alt Detector**\! Your contributions help make Discord a safer place for communities around the world.

We use **TypeScript (`.ts`)** files for our translations. You don't need to be a developer to help, but you must follow the structure below to ensure the bot continues to function correctly.

-----

## 🚀 How to Contribute

1.  **Fork** this repository.
2.  **Create a new file** named after your language code (e.g., `esES.ts`, `fr.ts`, `ja.ts`).
3.  **Copy the contents** of `enUS.ts` into your new file.
4.  **Update the Export Name**: Change the first line to match your language (e.g., `export const esES = {`).
5.  **Translate the values** (the text inside the quotes).
6.  **Submit a Pull Request** with a clear title like `feat: add Spanish translation`.

-----

## ⚠️ Translation Rules

### 1\. Keys vs. Values

The **Key** (left side) is what the code uses to find the text. The **Value** (right side) is what users see. **Only translate the Value.**

❌ **Incorrect** (The key was translated):

```typescript
error_de_sistema: "Se ha producido un error.", 
```

✅ **Correct** (Key stays English, Value is translated):

```typescript
error: "Se ha producido un error.",
```

### 2\. Placeholders `{variable}`

Words inside curly braces like `{user}`, `{guild}`, `{days}`, or `{latency}` are **placeholders**. The bot replaces these with real data automatically.

  * **Do not translate the word inside the brackets.**
  * You can move them within the sentence to fit your language's grammar.
  * **Example:** `Requested by {user}` ➡️ `{user} ha solicitado esto`.

### 3\. Markdown & Formatting

Alt Detector uses Discord Markdown. Please preserve:

  * `**text**` for **bold**.
  * `` `text` `` for `code blocks`.
  * `\n` represents a **new line**. Do not remove these.
  * `[Link Text]({url})` represents a clickable link. Only translate the "Link Text".

### 4\. Slash Command Constraints

Discord has strict rules for the `cmd` section:

  * **Command Names (`name`):** Must remain **lowercase**, with no spaces or special characters.
  * **Descriptions:** Keep these short (under 100 characters).

-----

## 🛠 File Structure Reference

| Section | Description |
| :--- | :--- |
| `common` | Basic terms used across the whole bot (Success, Loading, etc.). |
| `cmd` | Text for Slash Commands (names, descriptions, and responses). |
| `listeners` | Automatic messages sent during events (e.g., an Alt joining). |
| `quarantine` | Strings specifically for the manual review/quarantine system. |
| `time` | Unit labels for durations (day, hr, min, etc.). |

-----

## ✅ Final Checklist

  - [ ] My file is a `.ts` file.
  - [ ] My file starts with `export const [LanguageCode] = {`.
  - [ ] All my opening quotes `"` have matching closing quotes `"`.
  - [ ] Every line ends with a comma `,` (unless it's the last item in a block).
  - [ ] I have not changed any `{placeholder}` names.
  - [ ] All Slash Command `name` fields are lowercase.

**Need help?** Join our [Support Server](https://discord.com/invite/bRtYYHKZgt) and ask in the support channels\!
