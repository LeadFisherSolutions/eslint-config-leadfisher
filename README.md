# [Node js] ESLint config for leadfisher projects

## Usage

1. Install ESLint, this config and required plugins:

   ```bash
   npm i -D eslint eslint-plugin-import eslint-config-leadfisher
   ```

2. Add `"extends": "leadfisher"` to your `.eslintrc`.

3. Add following scripts

```json
{
  "scripts": {
    "lint": "eslint . && prettier --check \"**/*.js\" \"**/*.json\" \"**/*.md\" \".*rc\" \"**/*.yml\"",
    "fmt": "prettier --write \"**/*.js\" \"**/*.json\" \"**/*.md\" \".*rc\" \"**/*.yml\"",
    "test": "npm run -s lint"
  }
}
```

### Remove following lints, if you use different bandler than node or webpack

```json
{
  "new-cap": [
      "error",
      {
        "newIsCap": true,
        "capIsNew": false,
        "properties": true,
      },
    ],
    "import/no-unresolved": "off",
}
