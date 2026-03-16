# Create Mithril Application

This repo contains a simple `npx` tool to create a [mithril.js](https://mithril.js.org) application using Materialize CSS and TypeScript. Based on the NPX tutorial found [here](https://blog.shahednasser.com/how-to-create-a-npx-tool/).

It uses a [GitHub template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template), i.e. [this template](https://github.com/erikvullings/mithril-app), and replaces certain variables.

## Usage

```bash
npx create-mithrilts-app
```

## Template Variables

The following variables are replaced in the template files:

| Variable                  | Description                               | Example                    |
| ------------------------- | ----------------------------------------- | -------------------------- |
| `MITHRIL-APP-SHORT`       | Application short title (JSON string)     | `"MyApp"`                  |
| `MITHRIL-APP`             | Application title (JSON string)           | `"My Application"`         |
| `mithril-app`             | NPM package name (lowercase, hyphenated)  | `my-application`           |
| `APPLICATION_DESCRIPTION` | Application description (JSON string)     | `"A cool app"`             |
| `erikvullings`            | GitHub username / NPM scope (JSON string) | `"myusername"`             |
| `65533`                   | Development server port                   | `3000`                     |
| `@mithril-app/shared`     | Shared package import path                | `"@my-application/shared"` |

The tool prompts for:

1. **Project (folder) name** - Name of the directory to create (default: `create-mithril-app`)
2. **Application title** - Full title of your app (default: project name)
3. **Application short title** - Shorter version for UI (default: application title)
4. **Application description** - Description for package.json (default: empty)
5. **Webdev port** - Port for development server (default: `1234`)
