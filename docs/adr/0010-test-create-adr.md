# Test File Creation in ADR

* Status: accepted
* Date: 2024-09-23

## Context and Problem Statement

We need to test the creation of a new markdown file in the ADR structure. This test will help us verify if the GitHub and Azure APIs can handle creating files with specific content and structure.

## Considered Options

| Option                      | Pros                                      | Cons                                    |
|-----------------------------|-------------------------------------------|-----------------------------------------|
| Use GitHub API              |  Easy to use                              | Requires authentication               |
| Use Azure API               |  Scalable                                 | More complex setup                    |
| Manual Creation             |  Full control                             | Time-consuming                        |



## Decision Outcome

Chosen option: "Use GitHub API for file creation", because it allows automation of the process, which can be used in workflows and other CI/CD pipelines.

### Positive Consequences

| Consequence                                      |
|--------------------------------------------------|
| The process can be automated and integrated into workflows. |
| It helps in maintaining consistency and reduces manual errors. |

### Negative Consequences

| Consequence                                      |
|--------------------------------------------------|
| Requires correct permissions and access tokens.   |
| API rate limits can be a constraint in some cases. |
