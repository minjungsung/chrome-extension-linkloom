# NeatLink

Share the link. Skip the clutter.

Remove common tracking parameters from links before sharing. Preview every change and copy a cleaner URL in one click.

## Development

Open `chrome://extensions`, enable Developer mode, choose **Load unpacked**, and select `extension/`. No build or package dependencies are needed.

Run `npm test` for logic tests and `npm run package` to validate and create a clean ZIP in `dist/`.

## Privacy

See [PRIVACY.md](PRIVACY.md) for stored data and permission explanations. No accounts, analytics, ads, or developer servers.

## Support

Report bugs through this repository's issue tracker. Include reproducible steps and the extension version, with private information removed.

## License

MIT.

## Features and limits

NeatLink removes common tracking parameters before you share a URL. Paste a link or use the current tab, preview the cleaned result, and copy it.

FEATURES
- Remove UTM parameters and common click identifiers, including fbclid, gclid, and msclkid.
- See exactly which parameters were removed.
- Preserve unrelated query values and URL fragments.
- Keep detected signed or tokenized links unchanged.
- No automatic navigation changes, login, or tracking.

NeatLink works on HTTP and HTTPS URLs. It does not expand short links, visit the destination, or guarantee that a link contains no tracking. A cleaner URL does not change the privacy practices of the destination website. Check the preview before sharing important links.

PRIVACY
Links are processed locally and are not saved by the extension. Current-tab access happens only when you invoke the extension. The clipboard receives the cleaned link only when you choose Copy clean link. No developer servers or analytics.
