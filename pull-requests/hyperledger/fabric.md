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
                PR <a href="https://github.com/hyperledger/fabric/pull/3808" class=".btn">#3808</a>
            </td>
            <td>
                <b>
                    [WIP] Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test whether a new peer is able to reconcile from a purged peer

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 16:52:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3807" class=".btn">#3807</a>
            </td>
            <td>
                <b>
                    Revert "New Block Attestation Orderer GRPC service" & update protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 6c886cd9fc5b08df7b57c940c8793475edb14bec in release-2.5.

The Block Attestation service is targeted for Fabric v3.0, not Fabric v2.5.

This commit also updates to the latest fabric-protos-go v0.2.0 that is intended for Fabric v2.5 release.

Signed-off-by: David Enyeart [enyeart@us.ibm.com](mailto:enyeart@us.ibm.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 16:23:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3806" class=".btn">#3806</a>
            </td>
            <td>
                <b>
                    Update fabric-protos-go to v0.1.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fabric-protos-go v0.1.6 has been released for Fabric v2.4.x.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-23 15:43:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3804" class=".btn">#3804</a>
            </td>
            <td>
                <b>
                    remove sys-chan from e2e integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: Ib2a13c26ef48fedae5a69e5ee4c9bad95dfd56d3

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Removing system channel usage from integration tests

#### Related issues
Epic: #3511 
Issue: #3515 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 16:04:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3803" class=".btn">#3803</a>
            </td>
            <td>
                <b>
                    Add the domain parameter to the external service chain code parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description

When the chain code is deployed as an external service, the address may be an ip address rather than a domain.
So we need to add a domain field so that it can pass the TLS authentication.

<!--- Describe your changes in detail, including motivation. -->

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
        Created At 2022-11-21 12:17:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3802" class=".btn">#3802</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sufuy45 <yusuf.cagabey@gmail.com>

#### Type of change

- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 01:52:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3801" class=".btn">#3801</a>
            </td>
            <td>
                <b>
                    docs: make sentence more understandable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sufuy45 <yusuf.cagabey@gmail.com>

#### Type of change

- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 01:41:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3799" class=".btn">#3799</a>
            </td>
            <td>
                <b>
                    Remove usage of deprecated ioutils APIs
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

The commit removes usages of deprecated ioutils package APIs from the code base.

Signed-off-by: Artem Barger <artem@bargr.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-20 14:27:58 +0000 UTC
    </div>
</div>

