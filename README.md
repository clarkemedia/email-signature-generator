# Email Signature Generator

A free, open-source tool for creating professional HTML email signatures. No sign-up, no server, no tracking — runs entirely in your browser.

**[Try it live →](https://signatures.clarkemedia.ie)**

## Features

- **Fully customizable** — name, title, company, phone, email, website, address, logo, font, text size, accent colour, social links, buttons, and disclaimer
- **Live preview** — see changes instantly as you type
- **Tidy, collapsible form** — sections open one at a time so the preview stays in view
- **13 web-safe fonts and 4 text sizes** — from Arial and Calibri to Georgia and Garamond, in Small, Medium, Large or Extra Large
- **Address fields** — street, city, postcode/zip and country, shown on a single line
- **Light & dark mode preview** — check how your signature looks in both email themes
- **One-click copy** — copy as rich text (paste directly into your email client) or raw HTML
- **Conditional fields** — blank fields are automatically hidden from the output
- **Custom accent colour** — match your brand with the built-in colour picker
- **Adjustable logo size** — slider to keep the logo compact, especially on mobile
- **Social icons** — LinkedIn, Twitter/X, Facebook, Instagram, GitHub, YouTube, TikTok, Pinterest and WhatsApp, plus two custom icons for any other network (only shown when a URL is provided)
- **Call-to-action buttons** — add up to three clickable buttons side by side, each with its own text, link and colour (or one colour for all)
- **Customizable disclaimer** — edit the text or toggle it off entirely
- **Setup instructions** — step-by-step guides for Outlook (new, classic, Mac), Gmail, and Apple Mail
- **Zero dependencies** — single HTML file, no build step, no frameworks
- **Works offline** — download and open locally, no internet required (except for Google Fonts and social icons)

## How to Use

1. Open `index.html` in any modern browser (or visit the [live version](https://signatures.clarkemedia.ie))
2. Fill in your details — leave any field blank to hide it from the signature
3. Pick an accent colour to match your brand
4. Click **Copy signature** and paste into your email client
5. Follow the setup instructions for your specific email app

## Deploy Your Own

### GitHub Pages (free)

1. Fork this repository
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch** → `main` / `root`
4. Your signature generator will be live at `https://yourusername.github.io/email-signature-generator`

### Docker

```bash
docker run -d -p 8080:80 ghcr.io/clarkemedia/email-signature-generator:latest
```

Or with Docker Compose:

```bash
git clone https://github.com/clarkemedia/email-signature-generator.git
cd email-signature-generator
docker compose up -d
```

Then open `http://localhost:8080` in your browser.

The image is published for `linux/amd64`, `linux/arm64` and `linux/arm/v7`, so it also runs on Raspberry Pi and other ARM hosts.

### Self-hosted

Just serve `index.html` from any web server or CDN. It's a single file with no build step.

## Customizing the Defaults

The default field values in `index.html` showcase the creator's details as an example. To set your own defaults, edit the `value="..."` attributes on the form inputs near the top of the file.

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request. Some ideas:

- Additional email client instructions
- Image upload / base64 encoding for logos
- Colour theme presets
- Alternative signature layouts / templates
- i18n / localization

## License

MIT — see [LICENSE](LICENSE) for details.

## Credits

Created by [Eoin McMahon](https://clarkemedia.ie) at [Clarke Media](https://clarkemedia.ie).

Social icons provided by [Icons8](https://icons8.com).

---

If this tool saved you time, consider [buying me a coffee ☕](https://paypal.me/eoinmcm)
