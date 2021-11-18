# rabotaua/actions-dotnet-sonar

GitHub Action to persorm SonarCloud static code analysis for MSBuild projects

Sonar project will be automatically created and configured if needed with help of [rabotaua/actions-sonar-register](https://github.com/rabotaua/actions-sonar-register)

This action is for msbuild projects, if you have dotnet core project go here [rabotaua/actions-dotnet-sonar](https://github.com/rabotaua/actions-dotnet-sonar)

## Inputs

There are bunch of inputs which are documented in [action.yml](action.yml)

## Example usage

```yml
- uses: rabotaua/actions-msbuild-sonar@main
  with:
    sonar_token: ${{ secrets.SONAR_TOKEN }}
    github_token: ${{ secrets.GITHUB_TOKEN }}
    solution: 'MyProject.sln'
```
