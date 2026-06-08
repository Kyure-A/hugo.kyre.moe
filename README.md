# hugo.kyre.moe

Hugo site for `@kyremoe`, built with the local `hugo-twitter-style` theme.

## Preview

```sh
git submodule update --init
npm test
```

The preview server runs at `http://127.0.0.1:1314/`.

## Deployment

Pushes to `master` deploy to GitHub Pages through `.github/workflows/pages.yml`.

Set the repository's Pages source to GitHub Actions, then configure the custom domain as `hugo.kyre.moe`.

## Profile Data

The site uses static fallback values from `hugo.toml` and updates the profile client-side through FxTwitter:

```toml
[params]
xUsername = "kyremoe"
enableXDynamic = true
xProfileProxy = "https://api.fxtwitter.com/{username}"
```
