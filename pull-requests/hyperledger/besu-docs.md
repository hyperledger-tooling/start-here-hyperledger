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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    Document support for free gas networks when using London fee market
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Simon Dudley <simon.dudley@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Issue fixed

Fixes https://github.com/hyperledger/besu-docs/issues/1080

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

https://hyperledger-besu--1176.org.readthedocs.build/en/1176/private-networks/how-to/configure/free-gas/#4-enable-zero-base-fee-if-using-london-fork-or-later
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 11:15:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    Update estimated storage requirements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The documented storage requirements for a **full node** are incorrect.

I recently started my Besu experience by running a BONSAI node that unfortunately failed after The Merge, but its storage usage was just under 650GB when it was fully synced pre-merge (Linux, XFS filesystem)

I then synced using FOREST mode and was expecting 7TB of usage but it turned out to only be about 750GB. After speaking with @NicolasMassart (0x6E69636F#2619 on Discord) I was informed that the docs were wrong.

Please re-validate these numbers if you can. I have not had the time to run full Archive nodes to check those storage requirements, but they're likely correct.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 19:16:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    Add Warning to Docs about Restarting Node before Fully Syncing A Node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: gtrintinalia <gabriel.trintinalia@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Add Warning to Docs about Restarting Node before Fully Syncing A Node

## Issue fixed

fixes #1167

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
        Created At 2022-09-20 05:39:54 +0000 UTC
    </div>
</div>

