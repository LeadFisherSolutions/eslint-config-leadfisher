<h1 align="center">[Node js] ESLint config for leadfisher projects</h1>


**1**. Install ESLint, this config and required plugins: <br/>

   ```bash
   npm i -D eslint prettier eslint-plugin-import eslint-config-leadfisher eslint-config-prettier eslint-plugin-prettier
   ```

**2**. Add `"extends": ["leadfisher"]` to your `.eslintrc`.

**3**. _(optional)_ Add following scripts

```json
{
  "scripts": {
    "lint": "eslint . && prettier --check \"**/*.js\" \"**/*.json\" \"**/*.md\" \".*rc\" \"**/*.yml\"",
    "fmt": "prettier --write \"**/*.js\" \"**/*.json\" \"**/*.md\" \".*rc\" \"**/*.yml\"",
    "test": "npm run -s lint"
  }
}
```


<h2 align="center">Copyright & contributors</h2>

<p align="center">
Copyright © 2023 <a href="https://github.com/LeadFisherSolutions/eslint-config-leadfisher/graphs/contributors">Leadfisher contributors</a>.
Eslint-config-leadfisher is <a href="./LICENSE">MIT licensed license</a>.<br/>
Eslint-config-leadfisher is one of <a href="https://github.com/LeadFisherSolutions">leadfisher solutions</a>.
</p>
