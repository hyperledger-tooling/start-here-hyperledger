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
                PR <a href="https://github.com/hyperledger/fabric/pull/3243" class=".btn">#3243</a>
            </td>
            <td>
                <b>
                    Bump gorilla/handlers 1.4.0 to 1.5.1
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


- Improvement (improvement to code, performance, etc)


#### Description

<!--- Describe your changes in detail, including motivation. -->

Update gorilla/handlers dependency

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
        Created At 2022-02-21 03:33:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3242" class=".btn">#3242</a>
            </td>
            <td>
                <b>
                    Ignore expired CA/TLS CA certs on msp init (#3238)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ana Maria Franco <afrancoc2000@gmail.com>

Adding this line guarantees that expired CA certificates wont prevent orderer initialization as happened in [Issue #3238](https://github.com/hyperledger/fabric/issues/3238)

#### Type of change

- Bug fix

#### Description

Adding this line guarantees that expired CA certificates wont prevent orderer initialization as happened in [Issue #3238](https://github.com/hyperledger/fabric/issues/3238)


#### Related issues

[Issue #3238](https://github.com/hyperledger/fabric/issues/3238)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-20 21:23:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3237" class=".btn">#3237</a>
            </td>
            <td>
                <b>
                    Fix firewall warnings for integration tests on Mac
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When running integration tests locally on MacOS, each test causes a number of popup boxes containing the text
‘Do you want the application “peer” to accept incoming network connections?”.
Although this can be ignored, each popup takes the (cursor) focus away from the current window, and so is annoying when trying to do anything else.
This is caused because each test is launching one or more peer instances which get compiled on demand and appears to the firewall as a new executable.
The fix for this is to ensure that all listen addresses are explicitly set as localhost.  In this case, the chaincodeListenAddress host can be set to 127.0.0.1 rather than 0.0.0.0

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 11:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3235" class=".btn">#3235</a>
            </td>
            <td>
                <b>
                    Gateway support for mutual TLS networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support client authentication (mTLS), the gateway needs to pass the host peer’s client certificate when making connections to the other nodes in the network.
If client authentication is not enabled, then these certs will be ignored.

Resolves #3234 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 12:10:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3233" class=".btn">#3233</a>
            </td>
            <td>
                <b>
                    remove commercial paper references (backport #3232)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3232 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 20:15:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3232" class=".btn">#3232</a>
            </td>
            <td>
                <b>
                    remove commercial paper references
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

Remove all "Commercial Paper" tutorials and references from 2.4 doc.

#### Type of change

- New feature
- Documentation update

#### Description

Remove commercial paper tutorial - because it uses the prior dev apps method, not the new 2.4 Fabric Gateway method.

#### Release Note

Should add a comment to next release notes to use the Asset Transfer tutorial for 2.4 Fabric instead of Commercial Paper.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 15:41:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3230" class=".btn">#3230</a>
            </td>
            <td>
                <b>
                    doc - add new gateway to key concepts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

#### Type of change

- Documentation update

#### Description

New Fabric Gateway service page needed a link in Key Concepts page / list
(gateway.md)

#### Additional details

Add to go here near the bottom (logical sequential) - https://hyperledger-fabric.readthedocs.io/en/latest/key_concepts.html


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 19:42:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3229" class=".btn">#3229</a>
            </td>
            <td>
                <b>
                    Fix inconsistent behavior of GetBookmarkAndClose method in different statedb
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

- Bug fix

#### Description

<!--- Describe your changes in detail, including motivation. -->
When there are no more results in paginated range query, statecouchdb return endKey
as bookmark in GetBookmarkAndClose method, but stateleveldb return empty string as bookmark.
This inconsistent behavior may cause different code logic when use bookmark in smart contract
with different statedb.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 10:22:14 +0000 UTC
    </div>
</div>

