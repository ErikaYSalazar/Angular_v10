#Getting started with Angular

## Prerequisites

Install [Node.js](https://nodejs.org/en/download/)
Install angular cli `npm run install -g @angular/cli`
Create project `ng new angular10-app`. This project was generated without routing and with SASS.

## Thinks to know

- You get basic commads from [default README file](docs/README.md)
- Typescript is installed by default.

## Things to do

### Setup prettier

1. install prettier `npm install --save-dev prettier tslint-config-prettier`
2. added to tslint.json

```
{
  "extends": [
      "tslint:recommended",
      "tslint-config-prettier"
  ],
  ...
}
```

3. Configure prettier example [.prettierrc.json](.prettierrc.json)
4. Add pre-commit hook to re-format files that are marked as “staged” via git add before you commit.

- Install Husky `npm install --save-dev pretty-quick husky``
- Add to package.json

```
{
  "husky": {
    "hooks": {
      "pre-commit": "pretty-quick --staged"
    }
  }
}
```

RECOMENDATION: On VSCode check setting "Format on Save". Set Prettier as default.
