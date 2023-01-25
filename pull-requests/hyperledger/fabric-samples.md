---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    Add in 2.5 java test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 11:05:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/916" class=".btn">#916</a>
            </td>
            <td>
                <b>
                    Bump cookiejar from 2.1.2 to 2.1.4 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [cookiejar](https://github.com/bmeck/node-cookiejar) from 2.1.2 to 2.1.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/bmeck/node-cookiejar/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cookiejar&package-manager=npm_and_yarn&previous-version=2.1.2&new-version=2.1.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 06:22:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    Run FSAT tests with 2.5 images, binaries, and trigger on all builds for regression coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR runs the FSAT tests for all commits, not just edits under the full-stack-asset-transfer guide sub-folder.

We had some regressions in the fabric-shim when moving to 2.5.1 which would have been caught by the FSAT tests, had they been run with all of the samples commits.  This PR re-enables the FSAT tests to run on all builds: 

- runs with 2.5 binaries/ images 
- pins fabric-contract-api and fabric-shim to 2.4.0 (still some issues to sort out with 2.5.1) 
- Removes an annoying lint warning for unused variables.
- Displays a useful message to the console, explaining why Bananaman can not transfer a token to Appleman.   (In some cases of users running through the workshop, it was not clear that there was work to be done to implement this one-line function.)

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 16:15:35 +0000 UTC
    </div>
</div>

