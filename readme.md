# ⚡︎ @MODULE_NAME@

```
|:------------------------------------------------------:|
| ⚡︎ B o x L a n g ⚡︎
| Dynamic : Modular : Productive
|:------------------------------------------------------:|
```

<blockquote>
	Copyright Since 2023 by Ortus Solutions, Corp
	<br>
	<a href="https://www.boxlang.io">www.boxlang.io</a> |
	<a href="https://www.ortussolutions.com">www.ortussolutions.com</a>
</blockquote>

<p>&nbsp;</p>

@MODULE_DESCRIPTION@

---- 

This template can be used to create Ortus based BoxLang Modules written in BoxLang. To use, just click the `Use this Template` button in the github repository: https://github.com/ortus-boxlang/boxlang-module-template-bx and run the setup task from where you cloned it.

```bash
boxlang SetupTemplate.bx
```

The `SetupTemplate` task will ask you for your module name, id and description and configure the template for you! Enjoy!

## Directory Structure

Here is a brief overview of the directory structure:

-   `.github/workflows` - These are the github actions to test and build the module via CI
-   `.vscode` - VScode additions
-   `bifs` - Where you can code Built in Functions for BoxLang
-   `components` - Where you can code BoxLang components
-   `interceptors` - Where you can code BoxLang interceptors
-   `lib` - Place any Jar's or classes for your module that will be class loaded for you
-   `models` - Any models available to the runtime using `bxModules.{mapping}.models` path
-   `.cfformat.json` - A format config using the Ortus Standards
-   `.editorconfig` - Smooth consistency between editors
-   `.gitattributes` - Git attributes
-   `.gitignore` - Basic ignores. Modify as needed.
-   `.markdownlint.json` - A linting file for markdown docs
-   `box.json` - The box.json for your module used to publish to ForgeBox
-   `changelog.md` - A nice changelog tracking file
-   `CONTRIBUTING.md` - A contribution guideline
-   `ModuleConfig.bx` - Your module's configuration file
-   `readme.md` - Your module's readme. Modify as needed.

## Local Building

If you want to build the module, you can use `boxlang Build.bx` to build the module.  Here are the options you can pass to the script:

| Option      | Required | Default Value | Description                                  |
|-------------|----------|---------------|----------------------------------------------|
| `projectName` | Yes      | N/A           | The name of the project.                   |
| `version`   | No       | `1.0.0`       | The version of the module.                   |
| `branch`    | No       | `development` | The branch being built.                      |
| `buildId`   | No       | UUID (generated) | A unique identifier for the build.         |

```bash
boxlang Build.bx --projectName=MyModule --version=1.1.0
```

## Github Actions Automation

The Github actions will clone, test, package, and deploy your module to ForgeBox and the Ortus S3 accounts for API Docs and Artifacts. Please make sure the following environment variables are set in your repository.

> Please note that most of them are already defined at the org level

-   `FORGEBOX_TOKEN` - The Ortus ForgeBox API Token
-   `AWS_ACCESS_KEY` - The travis user S3 account
-   `AWS_ACCESS_SECRET` - The travis secret S3

> Please contact the admins in the `#infrastructure` channel for these credentials if needed

## Ortus Sponsors

BoxLang is a professional open-source project and it is completely funded by the [community](https://patreon.com/ortussolutions) and [Ortus Solutions, Corp](https://www.ortussolutions.com). Ortus Patreons get many benefits like a cfcasts account, a FORGEBOX Pro account and so much more. If you are interested in becoming a sponsor, please visit our patronage page: [https://patreon.com/ortussolutions](https://patreon.com/ortussolutions)

### THE DAILY BREAD

> "I am the way, and the truth, and the life; no one comes to the Father, but by me (JESUS)" Jn 14:1-12
