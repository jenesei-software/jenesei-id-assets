# Jenesei ID Assets

Public Jenesei ID assets available through the [jsDelivr](https://www.jsdelivr.com/) CDN.

## Usage

### Using a function

```ts
const ICON_VERSION = 'v1.3.0';

export function getSpriteUrl(props: { type: string }) {
  return `https://cdn.jsdelivr.net/gh/jenesei-software/jenesei-id-assets@${ICON_VERSION}/icons/${props.type}.svg`;
}
```

Example:

```ts
const logoUrl = getSpriteUrl({ type: 'logo' });
```

### Using a direct URL

```text
https://cdn.jsdelivr.net/gh/jenesei-software/jenesei-id-assets@v1.3.0/icons/logo.svg
```

For example, in HTML:

```html
<img
  src="https://cdn.jsdelivr.net/gh/jenesei-software/jenesei-id-assets@v1.3.0/icons/logo.svg"
  alt="Jenesei ID"
/>
```

## Available assets

- `checkbox`
- `id`
- `loading`
- `logo`

To use a different asset, replace `logo` in the URL or pass the required asset name as `type`.

Use a specific version such as `v1.3.0` to prevent future repository changes from unexpectedly affecting your application.
