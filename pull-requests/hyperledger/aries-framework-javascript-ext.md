---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    feat: add redux-store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!---
Provide a general summary of your changes in the Title above
-->

## Description

<!--- Describe your changes in detail -->

Add initial move to extensions repo. Adds redux-store with mostly the same structure as AFJ. Main difference is that we're not using lerna, and we're also not using the same version strategy. It makes more sense to me to be able to separately develop packages.

I've had some struggles to be able to create releases, update versions etc to the main branch from within a CI script. So I've tested out a new approach that I think could work really well.

We keep PRs open for all packages and once we merge them a new release will be created based on conventional commits. This means we do need to follow conventional commits, but also means we have an easy way to publish packages. This is an open source tool from google, and is completely automated using Github actions.

See https://github.com/TimoGlastra/aries-framework-javascript-ext/pull/2 for an example

- [x] Tests for the changes have been added (for bug fixes / features)
- [x] The commit message(s) follow [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [x] Documentation has been added / updated (for bug fixes / features)
- [x] Changes follow the **[contributing](../CONTRIBUTING.md)** document.

## Does this PR introduce a breaking change?

- [ ] Yes
- [x] No

<!-- If this PR contains a breaking change, please describe the impact and migration path for existing applications below. Make sure to indicate commits with breaking changes by appending a `!` after the type/scope as described by the conventional commits guidelines -->

## Which merge strategy will you use?

<!-- This indicates to reviewers whether they need to check your commits are ready to be rebased on main or not. Squashing only requires the title of the PR to follow conventional commits guidelines. Rebasing requires all commits to follow conventional commits guidelines, but allows to introduce multiple changes within a single PR. If you don't know what this means, Squash is probably the way to go. -->

- [ ] Squash (REVIEW PR title)
- [x] Rebase (REVIEW commit messages)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-28 11:55:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Add CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 15:53:10 +0000 UTC
    </div>
</div>

