# NewAperio GitHub Labels

This repo describes the way we set up GitHub labels for our projects at [NewAperio](https://newaperio.com). These are the labels we use with [Custodian](https://github.com/newaperio/custodian), our GitHub bot. The JSON files are designed to be used with [git-labelmaker](https://github.com/himynameisdave/git-labelmaker).

## Usage

*Note:* This step is only necessary if it's a repo *not* under our organization. The repos in our organization get these labels by default.

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

## Labels

These are the labels we use on repos that contain the main working code for our projects.

Since we don't use GitHub for project management, the labels only describe Pull Request statuses.

| Name             | Color      | Description                                                                     |
|------------------|------------|---------------------------------------------------------------------------------|
| `blocked`        | orange     | Signals an issue is blocked by extenuating circumstances                        |
| `in-progress`    | purple     | Denotes an issue actively being worked on; applied by Custodian                 |
| `needs-review`   | yellow     | Denotes a PR that is finished and is awaiting peer review; applied by Custodian |
| `question`       | magenta    | Signals a stalled issue because of outstanding question(s)                      |
| `ready-to-merge` | green      | Denotes a PR that has been reviewed and approved; applied by Custodian          |

## License

This repo is Copyright © 2017 NewAperio. It is free software, and may be
redistributed under the terms specified in the [LICENSE](/LICENSE.md) file.

## About NewAperio

This repo was written by NewAperio, LLC.

NewAperio is a web and mobile design and development studio. We offer [expert
software design and development][services] as part of our portfolio of services.
[Get in touch][contact] to see how our team can help you.

[services]: https://newaperio.com/services?utm_source=github
[contact]: https://newaperio.com/contact?utm_source=github
