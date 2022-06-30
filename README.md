# Available Workflows
Curated Reusable Workflows - see @gitadmin for updates to these workflows.


- ### Super Linter
The super-linter finds issues and reports them to the console output. Fixes are suggested in the console output but not automatically fixed, and a status check will show up as failed on the pull request. Full language linting is performed unless specifed. 

_This action runs on Metro_ (self-hosted vm)

Example:
```
  linter:
    uses: ocpdude/reusable/.github/workflows/linter.yaml@main
    with:
      language: java, javascript # Optional
```
Supported languages/linters: https://github.com/marketplace/actions/super-linter#supported-linters

- ### CodeQL Scanning
Inspect your codebase for quality and vunerabilites with CodeQL. Security vulnerabilities, bugs, and other errors are modeled as queries that can be executed against databases extracted from code. Full language analysis is performed unless specified.

_This action runs on Metro_ (self-hosted vm)

Example:
```
  codeql:
    uses: ocpdude/reusable/.github/workflows/codeql.yaml@main
    with:
      language: java # Optional
```
