# docs

Source for the public site **https://kesa-md.github.io/docs/**, which hosts the documentation and privacy policies for Kesa browser extensions. Extension stores link to the privacy policy pages here.

GitHub Pages builds the site with Jekyll from the default branch.

## Adding an extension

1. Create a folder named after the extension, for example `my-extension/`.
2. Add `index.md` with the documentation (front matter `permalink: /my-extension/`).
3. Add `privacy.md` with the privacy policy (front matter `permalink: /my-extension/privacy/`).
4. Add the extension to the `extensions` list in `_config.yml`, and to `header_pages` if it should appear in the site header.

The privacy policy address to give the store is `https://kesa-md.github.io/docs/<folder>/privacy/`.
