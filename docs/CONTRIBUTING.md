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
- Deployment is done using a custom GitHub Actions workflow which builds the app using Gatsby and commits it to the `gh-pages` branch where it is published by GitHub. It is based on the [GitHub Pages Action] plugin by Shohei Ueda. See [main.yml](.github/workflows/main.yml) for more details

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
