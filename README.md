# TypeScript Frontend Extension Pack

An opinionated selection of popular VS Code extensions for a TypeScript frontend.

Marketplace Link: https://marketplace.visualstudio.com/items?itemName=lukedavis.typescript-frontend-extension-pack

## Extensions

**Linting/Formatting**

- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

**Developer Environment**

- [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)

**In-File**

- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
  - When editing a tag name, it will edit the closing tag's name as well. Useful for renaming elements.
- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
  - My favorite spell checker, also supports multiple languages.
- [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
  - Displays the import size of your imports next to them. Incredibly useful to stay aware of bundle size.
- [Tailwind CSS Intellisense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)

## Quickstart

In order to make the most out of this extension pack, you will need to set up a few things on your project. Feel free to skip a section if you already have it set up.

### ESLint (JS/TS Linter)

If you aren't familiar with ESLint, I would advise reading up on [ESLint](https://eslint.org/) and it's package for TypeScript applications, [typescript-eslint](https://typescript-eslint.io/).

**Setup**

Create an ESLint config file in the root of your project. If using TypeScript, follow [this quickstart guide](https://typescript-eslint.io/getting-started#quickstart) from typescript-eslint.

### EditorConfig

[EditorConfig](https://editorconfig.org/) is great for keeping general consistency across your codebase, especially with multiple developers.

**Setup**

Create a `.editorconfig` file in the root of your project. I recommend this basic setup to start:

```yml
root = true

[*.{js,jsx,ts,tsx}]
charset = utf-8
indent_style = space
indent_size = 2

[*]
end_of_line = lf
insert_final_newline = true
trim_trailing_whitespace = true
```

### Prettier (Code Formatter)

Although most are probably familiar with [Prettier](https://prettier.io/), I highly advise creating a [Prettier config file](https://prettier.io/docs/en/configuration.html) and customizing it to your taste if you haven't.

**Setup**

I recommend this basic starting configuration:

```json
{
  "singleQuote": true,
  "semi": true,
  "tabWidth": 2
}
```

Prettier with plugins can be incredibly powerful. These are the ones I use in my projects.

- `prettier-plugin-tailwindcss`
- `@ianvsprettier-plugin-sort-imports`
- `prettier-plugin-classnames`
- `@softonus/prettier-plugin-whitespace-remover`
- `@softonus/prettier-plugin-duplicate-remover`
- `prettier-plugin-merge`
