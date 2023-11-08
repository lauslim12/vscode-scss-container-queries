# VSCode SCSS Container Queries

To reproduce the issue of CSS Language Server in Visual Studio Code. This minimum reproducible example is intentionally made with Vite as it has in-built SCSS/Less support so we don't have to worry about build processes.

Relevant issue: [VSCode#197744](https://github.com/microsoft/vscode/issues/197744)

## Reproduction

To reproduce the problem, please do the following steps.

- Clone this repository.

```bash
git clone git@github.com:lauslim12/vscode-scss-container-queries.git
```

- Switch to this repository.

```bash
cd vscode-scss-container-queries
```

- Install dependencies.

```bash
yarn
```

- Run the application and open `localhost:5173`.

```bash
yarn dev
```

- Observe the font size, and then open `style.scss` in Visual Studio Code. You should see the following error in the semicolon after `cqw` and `cqh`.

```txt
expression expected scss(css-expressionexpected)
```
