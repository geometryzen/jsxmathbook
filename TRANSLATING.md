# Translating Pro Git (2nd Edition)

The translations are managed in a decentralized way. Each translation team maintains their own project. Each translation is in its own repository, the Pro Git team simply pulls the changes and builds them into the https://git-scm.com website when ready.

## General guidance for translating Pro Git

Pro Git is a book about a technical tool, therefore translating it is difficult compared to a non-technical translation.

The following are guidelines to help you on your way:
* Before you begin, read the whole Git Pro book in English, so that you're aware of the content, and are familiar with the style used.
* Ensure you have a good working knowledge of git, so that explaining the technical terms is doable.
* Stick to a common style and format for the translation.
* Be sure to read and understand the basics of [Asciidoc formatting](https://asciidoctor.org/docs/asciidoc-syntax-quick-reference/). Not following the asciidoc syntax can lead to problems with building/compilation of the pdf, epub and html files needed for the book.

## Translating the book to another language

### Helping with a existing project

* Check for an already existing project in the following table.
* Go to the project's page on GitHub.
* Open an issue, introduce yourself and ask where you can help.

| Language       | GitHub page     |
| :------------- | :------------- |
| العربية        | [geometryzen/jsxmathbook-ar](https://github.com/geometryzen/jsxmathbook-ar) |
| Беларуская     | [geometryzen/jsxmathbook-be](https://github.com/geometryzen/jsxmathbook-be) |
| български език | [geometryzen/jsxmathbook-bg](https://github.com/geometryzen/jsxmathbook-bg) |
| Čeština        | [geometryzen/jsxmathbook-cs](https://github.com/geometryzen-cs/jsxmathbook-cs) |
| English        | [geometryzen/jsxmathbook](https://github.com/geometryzen/jsxmathbook) |
| Español        | [geometryzen/jsxmathbook-es](https://github.com/geometryzen/jsxmathbook-es) |
| فارسی          | [jsxmathbook/jsxmathbook-fa](https://github.com/geometryzen/jsxmathbook-fa) |
| Français       | [geometryzen/jsxmathbook-fr](https://github.com/geometryzen/jsxmathbook-fr) |
| Deutsch        | [geometryzen/jsxmathbook-de](https://github.com/geometryzen/jsxmathbook-de) |
| Ελληνικά       | [geometryzen/jsxmathbook-gr](https://github.com/geometryzen/jsxmathbook-gr) |
| Indonesian     | [geometryzen/jsxmathbook-id](https://github.com/geometryzen/jsxmathbook-id) |
| Italiano   | [geometryzen/jsxmathbook-it](https://github.com/geometryzen/jsxmathbook-it) |
| 日本語   | [geometryzen/jsxmathbook-ja](https://github.com/geometryzen/jsxmathbook-ja) |
| 한국어   | [geometryzen/jsxmathbook-ko](https://github.com/geometryzen/jsxmathbook-ko) |
| Македонски | [geometryzen/jsxmathbook-mk](https://github.com/geometryzen/jsxmathbook-mk) |
| Bahasa Melayu| [geometryzen/jsxmathbook-ms](https://github.com/geometryzen/jsxmathbook-ms) |
| Nederlands | [geometryzen/jsxmathbook-nl](https://github.com/geometryzen/jsxmathbook-nl) |
| Polski | [jsxmathbook-pl/jsxmathbook-pl](https://github.com/geometryzen2-pl/jsxmathbook-pl) |
| Português (Brasil) | [geometryzen/jsxmathbook-pt-br](https://github.com/geometryzen/jsxmathbook-pt-br) |
| Русский   | [geometryzen/jsxmathbook-ru](https://github.com/geometryzen/jsxmathbook-ru) |
| Slovenščina  | [geometryzen/jsxmathbook-sl](https://github.com/geometryzen/jsxmathbook-sl) |
| Српски   | [geometryzen/jsxmathbook-sr](https://github.com/geometryzen/jsxmathbook-sr) |
| Svenska  | [geometryzen/jsxmathbook-sv](https://github.com/geometryzen/jsxmathbook-sv) |
| Tagalog   | [geometryzen/jsxmathbook-tl](https://github.com/geometryzen/jsxmathbook-tl) |
| Türkçe   | [geometryzen/jsxmathbook-tr](https://github.com/geometryzen/jsxmathbook-tr) |
| Українська| [geometryzen/jsxmathbook-uk](https://github.com/geometryzen/jsxmathbook-uk) |
| Ўзбекча  | [geometryzen/jsxmathbook-uz](https://github.com/geometryzen/jsxmathbook-uz) |
| 简体中文  | [geometryzen/jsxmathbook-zh](https://github.com/geometryzen/jsxmathbook-zh) |
| 正體中文  | [geometryzen/jsxmathbook-zh-tw](https://github.com/geometryzen/jsxmathbook-zh-tw) |

### Starting a new translation

If there is no project for your language, you can start your own translation.

Base your work on the first edition of the book, available [here](https://github.com/geometryzen/jsxmathbook). To do so:
 1. Pick the correct [ISO 639 code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for your language.
 1. Create a [GitHub organization](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/creating-a-new-organization-from-scratch), for example: `jsxmathbook-[your code]` on GitHub.
 1. Create a project `jsxmathbook`.
 1. Copy the structure of geometryzen/jsxmathbook (this project) in your project and start translating.

### Updating the status of your translation

On https://git-scm.com, the translations are divided into three categories. Once you have reached one of these levels, contact the maintainers of https://git-scm.com/ so that they can pull the changes.

| Category | Completion     |
| :------------- | :------------- |
| Translation started for | Introduction translated, not much else. |
| Partial translations available in | up to chapter 6 has been translated. |
| Full translation available in |the book is (almost) fully translated. |

## Continuous integration with GitHub Actions

GitHub Actions is a [continuous integration](https://en.wikipedia.org/wiki/Continuous_integration) service that integrates with GitHub. GitHub Actions is used to ensure that a pull-request doesn't break the build or compilation. GitHub Actions can also provide compiled versions of the book.

The configuration for GitHub Actions is contained in the `.github/workflows` directory, and if you bring in the `main` branch of the root repository you'll get them for free.
However, if you created your translation repo by _forking_ the root repo, there's an extra step you must complete (if you did not fork, you can skip this part).
GitHub assumes that forks will be used to contribute to the repo from which they were forked, so you'll have to visit the "Actions" tab on your forked repo, and click the "I understand my workflows" button to allow the actions to run.

## Setting up a publication chain for e-books

This is a technical task, please ping @david to get started with epub publication.
