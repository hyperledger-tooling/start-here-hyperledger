---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4636" class=".btn">#4636</a>
            </td>
            <td>
                <b>
                    Upgrade Docker Dependency to v20.10.27.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Move `github.com/docker/docker` to v20.10.27.

#### Additional details

This may be the last commit to v2.2, but it's definitely a good one.

#### Related issues
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 19:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4635" class=".btn">#4635</a>
            </td>
            <td>
                <b>
                    docs: fix grammer for ledger docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Fix grammer for ledger docs.

#### Additional details

NA
#### Related issues

NA


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 17:04:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4634" class=".btn">#4634</a>
            </td>
            <td>
                <b>
                    Re-add the RSA definitions to BCCSP - RSA implementation additional c…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BCCSP supported RSA in version 1.4. The Fabric CA is currently using the Fabric 1.4 dependency. It is necessary to move Fabric CA off of Fabric 1.4 dependencies since they are no longer maintained. Fabric 2.X does not support RSA, however the CA still needs to support RSA for any older but not expired certificates that may be in use by older netwo

Github:
https://github.com/hyperledger/fabric/issues/4625


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 23:27:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4632" class=".btn">#4632</a>
            </td>
            <td>
                <b>
                    Fix docs that link to .md files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docs should link to the .html file rather than the .md file in order to get resolved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 22:38:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4631" class=".btn">#4631</a>
            </td>
            <td>
                <b>
                    Add TLS passthrough and SANs info to TLS doc (backport #4568)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4568 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 16:13:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4630" class=".btn">#4630</a>
            </td>
            <td>
                <b>
                    refactor gateway bft test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The test is really short on time. 
But I decided not to increase the time, 
but to break the test into separate time intervals.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 14:21:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4629" class=".btn">#4629</a>
            </td>
            <td>
                <b>
                    Update documents to remove remaining descriptions on JIRA (backport #4628)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4628 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 14:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4628" class=".btn">#4628</a>
            </td>
            <td>
                <b>
                    Update documents to remove remaining descriptions on JIRA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch removes remaining descriptions regarding JIRA in the repository. Also, it includes minor improvements of docs.

#### Type of change

- Documentation update

#### Description
It seems the Hyperledger JIRA instance was sunset at the end of last year.
On the other hands, there are some remaining descriptions regarding JIRA in the repository.
So, this patch removes the remaining descriptions. Also, it includes some minor improvements of docs.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 06:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4627" class=".btn">#4627</a>
            </td>
            <td>
                <b>
                    Re-add the RSA definitions to BCCSP - RSA implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    BCCSP supported RSA in version 1.4. The Fabric CA is currently using the Fabric 1.4 dependency.
    It is necessary to move Fabric CA off of Fabric 1.4 dependencies since they are no longer maintained.
    Fabric 2.X does not support RSA, however the CA still needs to support RSA for any older but not expired certificates that may be in use by older netwo

    Github:
    https://github.com/hyperledger/fabric/issues/4625
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-20 16:19:34 +0000 UTC
    </div>
</div>

