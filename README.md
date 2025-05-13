# Django ToDo list

This is a to-do list web application with the basic features of most web apps, such as accounts/login, API, and interactive UI.

- CSS | [Skeleton](http://getskeleton.com/)
- JS  | [jQuery](https://jquery.com/)

## Summary

In this project, I extended the GitHub Actions workflow by adding Helm CI steps and Docker image publishing:

- Updated the repository with my DockerHub credentials using GitHub Secrets.

- Added a new helm-ci job to the workflow.

- Ensured that the repository is checked out only once per workflow run to optimize performance.

- The helm-ci job includes the following steps:

    - Downloads Helm-related artifacts.

    - Executes helm template to render the chart.

    - Runs helm lint to validate the chart.

    - Packages the Helm chart.

    - Uploads the chart package as a GitHub Actions artifact.