# 🤝 Contributing Guidelines

## Reporting Issues

Not a coder? See the [support resources](https://github.com/twocaretcat/.github/blob/main/docs/SUPPORT.md) for information on how to:

- request features
- report bugs
- ask questions
- report security vulnerabilities

## Finding Issues to Work On

Issues with the `🚦 ready` label are ready to be worked on. If you comment on an issue, I can assign it to you.

Issues with the `🚦 needs triage` label generally need some more information before they can be worked on, but if you
**start a discussion** about it or leave a comment on the issue, I can likely get it ready for you.

If an issue is unclear or you have any questions about how a feature should be implemented, reach out before making any
changes so we can discuss the best way to do it.

## Tech Stack

Here are some details about how the project is made for anyone who is looking to contribute or use this project as reference:

- The site is written with the [React] library and built with [Gatsby]
- All components and pages are written in [TypeScript], with config files written with JavaScript as required
- All components are written as functions and use hooks for additional React features
- [DaisyUI] component classes are used to style most components, with [Tailwind CSS] (via [PostCSS]) used for additional styling
- [PDF-LIB] is used to actually merge the input PDF documents in the browser
- Deployment is done using a custom GitHub Actions workflow which builds the app using Gatsby and commits it to the `gh-pages` branch where it is published by GitHub. It is based on the [GitHub Pages Action] plugin by Shohei Ueda. See [main.yml](../.github/workflows/main.yml) for more details

## Commands

We can build the site using the Gatsby CLI. All of the necessary commands are declared in `package.json` for convenience.

There are two ways to build & serve the site:

1. Use `bun run develop` to run the app in development mode. This will start the development server at [localhost:8000](https://localhost:8000) (by default). The project will automatically be rebuilt when changes are made, or

2. Use `bun run build` to generate a production build of the app, then use `bun run serve` to serve it. The site can be viewed at [localhost:9000](https://localhost:9000) (by default)

`bun run clean` can be used to clear the local Gatsby cache if you encounter any issues with stale data/dependencies

See the [Gatsby CLI docs](https://www.gatsbyjs.com/docs/reference/gatsby-cli/) for additional commands and options that you can run with `bunx gatsby COMMAND`

## License

By contributing to this project, you agree that your contributions will be licensed under the project license.

[Gatsby]: https://www.gatsbyjs.com/
[React]: https://reactjs.org/
[TypeScript]: https://www.typescriptlang.org/
[DaisyUI]: https://daisyui.com/
[Tailwind CSS]: https://tailwindcss.com/
[PostCSS]: https://postcss.org/
[PDF-LIB]: https://pdf-lib.js.org/
[Github Pages Action]: https://github.com/peaceiris/actions-gh-pages
