---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2977" class=".btn">#2977</a>
            </td>
            <td>
                <b>
                    ci(github): fix path filtering of required but skipped workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Migrated from the stock GitHub Actions yaml syntax to using this custom
action[1] that allows us to skip the running of jobs based on path filtering.
The difference compared to the old solution is that this one won't just
skip the checks that are marked as required but it will pass them instead.
2. This is a suboptimal solution because we have to run each job so that
the code can be checked out and then examined for changes. This uses
resources that we should not have to expend, but currently there's no way
to avoid this because of the way the GitHub handles required checks that
are skipped (which cause a deadlock on the CI at the currently).
3. There is a relevant discussion thread about the problem here [2] which
should be voted on heavily so that it gets the necessary attention from
the product teams at GitHub.

Quoting the relevant part of the GitHub documentation directly:

> Handling skipped but required checks
> Warning: If a workflow is skipped due to path filtering, branch
> filtering or a commit message, then checks associated with that workflow
> will remain in a "Pending" state. A pull request that requires those
> checks to be successful will be blocked from merging.
>
> For this reason you should not use path or branch filtering to skip
>  workflow runs if the workflow is required. For more information, see
>  "Skipping workflow runs" and "Required workflows."
>
> If, however, a job within a workflow is skipped due to a conditional,
> it will report its status as "Success". For more information, see
> "Using conditions to control job execution."

**Source** (link broken into multiple lines to avoid it being longer than
100 characters):

https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/
collaborating-on-repositories-with-code-quality-features/
troubleshooting-required-status-checks#handling-skipped-but-required-checks

[1] https://github.com/dorny/paths-filter
[2] https://github.com/orgs/community/discussions/44490

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 19:43:39 +0000 UTC
    </div>
</div>

