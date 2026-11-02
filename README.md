# Peach Black for Standard Notes

A CSS-only custom theme using near-black `#090909`, charcoal `#171717`, borders `#343434`, soft white `#F5F5F5`, muted text `#999999`, and warm peach `#FFC49A`.

## Install

1. Open Standard Notes **Preferences → Plugins**.
2. Under **Install Custom Plugin**, enter:

   `https://cdn.jsdelivr.net/gh/Lawsinex/standard-notes-peach-black-theme@v1.0.0/ext.json`

3. Confirm installation, then select **Peach Black** in **Preferences → Appearance → Themes** (or Quick Settings → Themes).

To switch back, select another theme. To remove, use **Preferences → Plugins → Manage Plugins**.

## Package

- `ext.json`: Standard Notes `SN|Theme` manifest.
- `theme.css`: native StyleKit and application variable overrides.
- `package.json`: desktop ZIP entry point (`sn.main`) and matching version.
- `v1.0.0` Git tag: fixed CSS version for reproducible installation.

No JavaScript, fonts, images, trackers, imports, or external asset references are included. The browser retrieves the manifest and stylesheet from jsDelivr/GitHub. The stylesheet does not request note access. Desktop clients can download the tagged source ZIP.

Fonts, text sizes, layout, and editing behavior remain controlled by Standard Notes. Error, success, and optional tag colors remain distinct. Third-party editors may apply their own styles. Mobile and native desktop appearance require separate verification.

## Color contrast

Body text, muted text, placeholders, and peach links meet WCAG AA text contrast on both primary backgrounds. Peach filled controls use near-black text. Borders are intentionally subtle, as in the reference image.

## Sources

- [Building a theme plugin](https://standardnotes.com/help/plugins/themes)
- [Publishing your plugin](https://standardnotes.com/help/plugins/publishing)
- [Standard Notes StyleKit colors](https://github.com/standardnotes/app/blob/main/packages/styles/src/Styles/_colors.scss)
- [Standard Notes application theme variables](https://github.com/standardnotes/app/blob/main/packages/web/src/stylesheets/_theme.scss)

## License

MIT — see LICENSE.
