# Test File Creation in ADR

* Status: accepted
* Date: 2024-09-23

## Context and Problem Statement

We need to test the creation of a new markdown file in the ADR structure. This test will help us verify if the GitHub and Azure APIs can handle creating files with specific content and structure.

## Considered Options

* Use GitHub API for file creation
* Use Azure API for file creation
* Manual file creation and commit

## Decision Outcome

Chosen option: "Use GitHub API for file creation", because it allows automation of the process, which can be used in workflows and other CI/CD pipelines.

### Positive Consequences

* The process can be automated and integrated into workflows.
* It helps in maintaining consistency and reduces manual errors.

### Negative Consequences

* Requires correct permissions and access tokens.
* API rate limits can be a constraint in some cases.
