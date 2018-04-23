# NewAperio GitHub Labels

This repo contains JSON files that describe the way we set up GitHub labels for our projects at [NewAperio](https://newaperio.com). These are the labels we use with [Custodian](https://github.com/newaperio/custodian), our GitHub bot. The JSON files are designed to be used with [git-labelmaker](https://github.com/himynameisdave/git-labelmaker).

## Usage

In a new repo, you probably want to first delete GitHub's default labels:

```bash
git-labelmaker # then select option 4 "Remove All Labels"
```

Then you can create labels using one of the sets here. Clone the repo and then run the command:

```bash
git-labelmaker # then select option 2 "Add Labels From Package"
               # provide *full* filepath to one of the JSON files
               # e.g. /Users/newaperio/code/github-labels/code.json
```

## Code

This label package is designed to be used on repos that contain the main working code for our projects. This can be an API or a frontend or a traditional HTML server app. This package has been used in Rails and Elixir projects.

| Name             | Color      | Category | Description                                                        |
|------------------|------------|----------|--------------------------------------------------------------------|
| `api`            | black      | focus    | Issues related to the API                                          |
| `blocked`        | orange     | status   | Signals an issue is blocked by extenuating circumstances           |
| `bug`            | red        | type     | Denotes an issue related to an existing bug                        |
| `database`       | black      | focus    | Issues related to data storage                                     |
| `documentation`  | black      | focus    | Issues related to documenting the code or API                      |
| `enhancement`    | light blue | type     | Denotes an issue that is an enhancement of existing functionality  |
| `feature`        | blue       | type     | Denotes a new feature that is planned for the app                  |
| `in-progress`    | purple     | status   | Denotes an issue actively being worked on                          |
| `infra`          | black      | focus    | Issues related to infrastructure, external services, or deployment |
| `needs-review`   | yellow     | status   | Denotes a PR that is finished and is awaiting peer review          |
| `question`       | magenta    | status   | Signals a stalled issue because of outstanding question(s)         |
| `ready-to-merge` | green      | status   | Denotes a PR that has been reviewed and approved                   |
| `testing`        | black      | focus    | Issues related to testing the app                                  |

## Docs

This label package is designed to be used on repos that contain documentation for our projects. This is traditionally an API Blueprint repo.

| Name             | Color      | Category | Description                                                        |
|------------------|------------|----------|--------------------------------------------------------------------|
| `blocked`        | orange     | status   | Signals an issue is blocked by extenuating circumstances           |
| `bug`            | red        | type     | Denotes an issue related to an existing bug                        |
| `enhancement`    | light blue | type     | Denotes an issue that is an enhancement of existing functionality  |
| `feature`        | blue       | type     | Denotes a new feature that is planned for the app                  |
| `in-progress`    | purple     | status   | Denotes an issue actively being worked on                          |
| `question`       | magenta    | status   | Signals a stalled issue because of outstanding question(s)         |
| `ready-to-merge` | green      | status   | Denotes a PR that has been reviewed and approved                   |
| `rfc`   | yellow     | status   | Denotes a PR that is finished and is awaiting peer review          |
