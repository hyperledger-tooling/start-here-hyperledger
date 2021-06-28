# Hyperledger Start Here

The repository contains the pages to be served. This repository is served
as a [website](https://start-here.hyperledger.org)
lists pull requests raised in last 7 days, new releases in the last 7 days
and easy to get started possible contribution opportunities at Hyperledger.

**Note:** This repository wouldn't require a manual PR for rendering
the contents served in the website. You would contribute here in case you
have a need to change the theme or layout of the project.

## Getting the latest backend

This repository uses `git submodule`. You will have to update the branch
name in the [.gitmodules](.gitmodules) file. If the branch has been updated
on the original repository and you would like to update a reference to it
then run the following command

```
git submodule update --remote
```

## Development

Run the following command, to host the site locally on your development
environment. Note that this requires `docker` and `docker-compose` tools.

```shell
docker-compose -f docker/docker-compose-test.yaml up --build
```

## Contributions

Each commit must include `Signed-off-by:`
in the commit message (run `git commit -s` to auto-sign).
This sign off means you agree the commit satisfies the
[Developer Certificate of Origin(DCO)](https://developercertificate.org/).
