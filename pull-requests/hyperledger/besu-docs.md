---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1067" class=".btn">#1067</a>
            </td>
            <td>
                <b>
                    remove context and branch cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

- Remove context from CI config as context was removed from Circle CI project config, making jobs fail.
- remove branch from cache key as it prevents it to be reused between
  branches when they could be similar most of the time.
  This was unnecessary zealous engineering.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

failing https://app.circleci.com/pipelines/github/hyperledger/besu-docs/4189/workflows/b247a0e6-2495-4177-8cf2-2c85a0f82a1e

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [ ] Documentation content
- [ ] Documentation page organization

For tool changes:

- [x] CircleCI workflow
- [ ] Build and QA tools (for example, lint or vale)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
- [ ] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 09:02:42 +0000 UTC
    </div>
</div>

