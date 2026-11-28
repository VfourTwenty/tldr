# glab ci

> Manage GitLab CI/CD pipelines and jobs.
> More information: <https://gitlab.com/gitlab-org/cli/-/blob/main/docs/source/ci/_index.md>.

- Watch the status of the latest pipeline on the current branch in real time:

`glab ci status {{[-l|--live]}}`

- List pipelines with a specific status:

`glab ci list {{[-s|--status]}} {{failed|running|success|...}}`

- Validate the `.gitlab-ci.yml` file in the current directory:

`glab ci lint`

- Display the fully merged CI/CD configuration with all `include` directives resolved:

`glab ci config compile`

- Run a new pipeline on a specific branch, passing a CI/CD variable:

`glab ci run {{[-b|--branch]}} {{branch_name}} --variables {{key}}:{{value}}`

- Stream the log of a specific job in real time:

`glab ci trace {{job_id|job_name}}`

- Retry a specific job:

`glab ci retry {{job_id|job_name}}`

- Interactively view, run, retry, and cancel the jobs of the latest pipeline on the current branch:

`glab ci view`
