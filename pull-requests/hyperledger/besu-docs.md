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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    Post-Merge doc updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

Update documentation around The Merge, including:

- Add a **Connect to a network** section under **Get started**, which includes:
  - **Sync Besu** - moved from the previous **How to > Connect to a network**
  - **Connect to Mainnet** - a new guide with specific instructions on connecting Besu to Mainnet with any consensus client.
  - **Connect to a testnet** - a new guide with specific instructions on connecting Besu to a testnet with any consensus client.
- Rename **How to > Connect to a network** to **How to > Find and connect to peers**.
- Add a **Run Besu and Teku on Mainnet** tutorial, similar to the existing testnet tutorial. These tutorials are similar to the get started guides, but include specific instructions for Teku.
- Edit terminology around The Merge from future to past tense, or remove such terminology in various pages.
- Add a note at the top of the **Prepare for The Merge** page. Eventually this page should be deleted and redirect to the connect to Mainnet guide.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1172 

## Impacted parts

- [x] Documentation content
- [x] Documentation page organization

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

Important pages to review:

- [Connect to Mainnet guide](https://hyperledger-besu--1173.org.readthedocs.build/en/1173/public-networks/get-started/connect/mainnet/)
- [Connect to a testnet guide](https://hyperledger-besu--1173.org.readthedocs.build/en/1173/public-networks/get-started/connect/testnet/)
- [The Merge conceptual page](https://hyperledger-besu--1173.org.readthedocs.build/en/1173/public-networks/concepts/the-merge/)
- [Run Besu and Teku on Mainnet tutorial](https://hyperledger-besu--1173.org.readthedocs.build/en/1173/public-networks/tutorials/besu-teku-mainnet/)
- [Run Besu and Teku on a testnet tutorial](https://hyperledger-besu--1173.org.readthedocs.build/en/1173/public-networks/tutorials/besu-teku-testnet/)

Some questions I still have:

1. Do we recommend setting `host-allowlist` and `engine-host-allowlist` to `*` on Mainnet? We currently recommend against this in the docs, but Discord users seem to all set them to `*`.
1. Does Teku require setting bootnodes for specific networks or are they set by default?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-17 02:42:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1171" class=".btn">#1171</a>
            </td>
            <td>
                <b>
                    Link from system requirements to jvm memory page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
- [ ] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 21:21:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1170" class=".btn">#1170</a>
            </td>
            <td>
                <b>
                    Distribute troubleshooting content
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

The troubleshooting/FAQ page was removed in the Besu docs restructure (#1085). This PR distributes the content from that page across the site on the relevant pages.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1098 

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] Github Actions workflow
- [ ] Build and QA tools configuration (for example, lint rules or Vale style)
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

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 20:36:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    use sha for weekly action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Signed-off-by: Nicolas MASSART <nicolas.massart@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Use Sha for action version (and allow it in github config) as the @v1 not working on this action.
Using commit sha is more secure anyway.

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

## Issue fixed


https://github.com/hyperledger/besu-docs/actions/runs/3052051159

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [ ] Documentation content
- [ ] Documentation page organization

For tool changes:

- [x] Github Actions workflow
- [ ] Build and QA tools configuration (for example, lint rules or Vale style)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

NA

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 10:33:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    remove circle ci config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Signed-off-by: Nicolas MASSART <nicolas.massart@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Remove the remains of Circle CI

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

## Issue fixed

fixes #1146 

<!-- Link to the GitHub issue that your PR addresses.

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
- [x] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview


NA

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 10:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1166" class=".btn">#1166</a>
            </td>
            <td>
                <b>
                    Combine/remove old content
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

Combine/remove content from pages that were omitted in the restructure.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1099 
fixes #1100 

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] CircleCI workflow
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

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 07:00:59 +0000 UTC
    </div>
</div>

