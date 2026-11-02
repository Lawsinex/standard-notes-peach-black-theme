# Peach Black for Standard Notes

A CSS-only custom theme using near-black `#090909`, charcoal `#171717`, borders `#343434`, soft white `#F5F5F5`, muted text `#999999`, and warm peach `#FFC49A`.

## Install

### Web app

1. Download `Peach-Black-Theme.sn.txt` from this repository.
2. Open Standard Notes **Preferences → Backups → Import backup**, and select that file.
3. Select **Peach Black** in **Preferences → Appearance → Themes** (or Quick Settings → Themes).

This is a Standard Notes version `004` import file containing exactly one `SN|Theme` item. It contains no notes, keys, account information, or application preferences. The item uses the same `package_info`, `area`, and `hosted_url` structure as the plugin installer. Activation is left to the user. Automatic updates are disabled; the stylesheet stays pinned to `v1.0.0`.

The web app observed on 2 November 2026 blocks jsDelivr manifest downloads through its Content Security Policy. Its external downloader also uses `credentials: include`, so raw GitHub's wildcard CORS response is rejected. The theme-only data import avoids that manifest download while the normal theme manager loads the CSS as a stylesheet. Browser protections stay enabled.

### Desktop plugin installer

Where the URL installer supports the endpoint, use **Preferences → Plugins → Install Custom Plugin** with:

`https://cdn.jsdelivr.net/gh/Lawsinex/standard-notes-peach-black-theme@v1.0.0/ext.json`

Then select **Peach Black** under **Appearance**. Native desktop installation has not been verified.

To switch back, select another theme. To remove, use **Preferences → Plugins → Manage Plugins**.

## Package

- `ext.json`: Standard Notes `SN|Theme` manifest.
- `theme.css`: native StyleKit and application variable overrides.
- `package.json`: desktop ZIP entry point (`sn.main`) and matching version.
- `Peach-Black-Theme.sn.txt`: theme-only package for the built-in data importer.
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
