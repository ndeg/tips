# Makefile tips

A Makefile can be used to group commands and improve developer experience. It can also be used with CI/CD.

By convention, the Makefile` file should be created on the root folder of your project.

Also, commands should be consistent between your different projects, in order to ease project switching.
Project specificities must be avoided.

Here's a proposal for a Makefile used for a web application.

Please note that indentation between keyword and the commands must be a tabulation.

```makefile
install: ## Installs the projects
	echo 'Application installed'
	echo 'Application started'

start: ## Starts the application
	echo 'Application started'

stop: ## Stops the application
	echo 'Application stopped'

watch: ## Launches the application with live refresh
	echo 'Application launched in watch mode.

uninstall: ## Uninstalls the application
	echo 'Application uninstalled'

cli: ## Goes to the command line interface of the main application 
    echo 'Welcome to the CLI.'
    
db: ## Goes to the command line interface of the application's databasse.
    echo 'Welcome to the database CLI.'

unit-test: ## Tests the application with unit testing
	echo 'Application unit tested.'

functional-test: ## Tests the application with functional testing
	echo 'Application unit tested.'

static-analysis: ## Analyses the code of the application.
	echo 'Application unit tested.'

coding-standard-fix: ## Applies coding standards.
	echo 'Code beautified'

coding-standard-check: ## Checks if the coding standard has been respected.
	echo 'Coding standards checked'

.PHONY: help
help: ## Shows this help
		@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'

.DEFAULT_GOAL := help
```

[Back to index](../../README.md)
