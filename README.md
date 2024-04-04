# Finalyze with CodeQL

Performs the actual SAST analysis with previously initialized CodeQL. Leverages the official [CodeQL: Finish action](https://github.com/github/codeql-action/blob/main/analyze/action.yml).

> This action is part of the Codebelt ecosystem and ensures a consistent way of: 
> 
> - Defining your CI/CD pipeline 
> - Structuring your repository
> - Keeping your codebase small and feasible
> - Writing clean and maintainable code
> - Deploying your code to different environments
> - Automating as much as possible
>
> A paved path to excel as a DevSecOps Engineer.

## Usage

To use this action in your GitHub repository, you can follow these steps:

```yaml
uses: codebeltnet/codeql-scan-finalize@main
```

### Inputs

This action has no inputs.

### Outputs

This action has no outputs.

## Examples

### Complete CodeQL SAST Analysis

```yaml
steps:
  - name: Prepare CodeQL SAST Analysis
    uses: codebeltnet/codeql-scan@main

  - name: Build
    uses: codebeltnet/dotnet-build@main
    with:
      uploadBuildArtifact: false

  - name: Finalize CodeQL SAST Analysis
    uses: codebeltnet/codeql-scan-finalize@main
```

## Contributing to Finalyze with CodeQL

Contributions are welcome! 
Feel free to submit issues, feature requests, or pull requests to help improve this action.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
