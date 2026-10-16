# LinkLoom

Clean once. Share anywhere.

LinkLoom prepares a single URL or an entire list for sharing. Remove common tracking parameters, review the changes, and copy clean links as plain text or a Markdown list.

## Features

- Process up to 100 links at once, one URL per line.
- Remove UTM parameters and common click identifiers such as fbclid, gclid, and msclkid.
- Preview the resulting links and the removed parameters.
- Keep detected signed or tokenized URLs unchanged.
- Copy plain URLs or Markdown links, or export a text file.
- Use the current tab without permanent website access.

## Limits

LinkLoom does not visit destinations, expand short URLs, or guarantee that all tracking is removed. It preserves unrelated query values and fragments. Invalid links are excluded from copy/export results. Links with embedded credentials are rejected. Always review important links before sharing.

## Development

Open `chrome://extensions`, enable Developer mode, choose **Load unpacked**, and select `extension/`. All runtime assets are packaged locally.

Run `npm test` for logic tests. Run `npm run package` to validate and create an upload ZIP in `dist/`. No build step or runtime package dependencies are required.

## Privacy

URLs are held in popup memory only and are not persistently stored. Links are placed on the clipboard or in a downloaded text file only at your request.

`activeTab` reads the current tab URL and title only when you invoke the extension and choose Current tab. No page content is read.

See [PRIVACY.md](PRIVACY.md). No developer servers, advertising, or analytics.

## Support

Report reproducible bugs through this repository's issue tracker. Remove private information first.

## License

MIT.
