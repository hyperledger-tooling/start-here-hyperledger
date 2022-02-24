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
                PR <a href="https://github.com/hyperledger/fabric/pull/3256" class=".btn">#3256</a>
            </td>
            <td>
                <b>
                    Update go.mod version to 1.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The go version directive in go.mod indicates the minimum version of Go that the module works with.
Since Fabric is no longer tested with Go 1.14, it is not known whether Go 1.14 would still
be compatible with current Fabric.
Therefore this commit updates the go directive to 1.17, which is the current version
of Go that Fabric is tested against.

Keeping the go directive up to date with the tested version of go will also
eliminate confusion from users about the recommended version of go.

Note that with the 1.17 version, go.mod has a new format and includes all
indirect depenendencies in a second require stanza.
1.17 also removes go.mod and go.sum from the vendor directories.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 06:21:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3255" class=".btn">#3255</a>
            </td>
            <td>
                <b>
                    Ignore expired CA/TLS CA certs on msp init (#3238) (backport #3249)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3249 done by [Mergify](https://mergify.com).


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
        Created At 2022-02-24 06:00:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3254" class=".btn">#3254</a>
            </td>
            <td>
                <b>
                    [FAB-18429] ledgerutil: Add 'identifytxs' subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature

#### Description

This patch adds a new subcommand to ledgerutil that traverses transactions in a specified ledger and outputs transaction information (write sets) as a JSON file.
The information is intended to be used to identify a causal transaction when two ledgers of the same channel are found to be different.

#### Additional details

Although the tests and documentations are incomplete, first I'd like to have comments about whether this patch matches what is originally intended and expected when the issue #2979 is created.

The current output JSON (reformatted) would be like
```json
{
  "ledgerid": "mychannel",
  "blocks": [
    {
      "number": 0,
      "transactions": []
    },
    {
      "number": 1,
      "transactions": []
    },
    {
      "number": 2,
      "transactions": []
    },
    {
      "number": 3,
      "transactions": [
        {
          "id": "1212bce58dfb121f0fe4c43cee8e043001698c3e115eb908058f0984bc4fb658",
          "timestamp": "1633074375.833477438",
          "writes": []
        }
      ]
    },
    {
      "number": 4,
      "transactions": [
        {
          "id": "d492e054e7f62380897b4a3b618400312a6b5f1886cc8f88b34fd6d7797255c5",
          "timestamp": "1633074384.429622751",
          "writes": []
        }
      ]
    },
    {
      "number": 5,
      "transactions": [
        {
          "id": "79e9bdefb71a5c00efe239ba7c45b5ae2f89a7841c73591fc060701ea6612399",
          "timestamp": "1633074392.873929810",
          "writes": [
            {
              "namespace": "_lifecycle",
              "isDelete": false,
              "key": "6e616d657370616365732f6669656c64732f6661626361722f436f6c6c656374696f6e73",
              "value": "1200"
            },
            {
              "namespace": "_lifecycle",
              "isDelete": false,
              "key": "6e616d657370616365732f6669656c64732f6661626361722f456e646f7273656d656e74496e666f",
              "value": "120b0a013110011a0465736363"
            },
            {
              "namespace": "_lifecycle",
              "isDelete": false,
              "key": "6e616d657370616365732f6669656c64732f6661626361722f53657175656e6365",
              "value": "0801"
            },
            {
              "namespace": "_lifecycle",
              "isDelete": false,
              "key": "6e616d657370616365732f6669656c64732f6661626361722f56616c69646174696f6e496e666f",
              "value": "122a0a0476736363122212202f4368616e6e656c2f4170706c69636174696f6e2f456e646f7273656d656e74"
            },
            {
              "namespace": "_lifecycle",
              "isDelete": false,
              "key": "6e616d657370616365732f6d657461646174612f666162636172",
              "value": "0a13436861696e636f6465446566696e6974696f6e120853657175656e6365120f456e646f7273656d656e74496e666f120e56616c69646174696f6e496e666f120b436f6c6c656374696f6e73"
            }
          ]
        }
      ]
    }
  ]
}
```

#### Related issues

#2979 and https://jira.hyperledger.org/browse/FAB-18429
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 00:28:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3253" class=".btn">#3253</a>
            </td>
            <td>
                <b>
                    Ignore expired CA/TLS CA certs on msp init (#3238) (backport #3249)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3249 done by [Mergify](https://mergify.com).


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
        Created At 2022-02-23 08:41:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3252" class=".btn">#3252</a>
            </td>
            <td>
                <b>
                    Ignore expired CA/TLS CA certs on msp init (#3238) (backport #3249)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3249 done by [Mergify](https://mergify.com).


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
        Created At 2022-02-23 08:41:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3249" class=".btn">#3249</a>
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
                Adding this line guarantees that expired CA certificates wont prevent orderer initialization as happened in https://github.com/hyperledger/fabric/issues/3238

#### Type of change
Bug fix

#### Description
Adding this line guarantees that expired CA certificates wont prevent orderer initialization as happened in https://github.com/hyperledger/fabric/issues/3238

#### Related issues
https://github.com/hyperledger/fabric/issues/3238
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 13:29:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3248" class=".btn">#3248</a>
            </td>
            <td>
                <b>
                    Gateway support for mutual TLS networks (backport #3235)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3235 done by [Mergify](https://mergify.com).


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
        Created At 2022-02-22 13:22:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3245" class=".btn">#3245</a>
            </td>
            <td>
                <b>
                    Fix Orderer test flake #3149
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #3149  In case of accumulated bytes since last snapshot 
exceed limit while taking snapshot check whether the pb buffer
type is of raftpb.EntryNormal, since blocks are marshalled into 
pb buffers of raftpb.EntryNormal and not raftpb.EntryConfChange

Signed-off-by: Shivdeep Singh <Shivdeep.Singh@ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-22 10:30:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3244" class=".btn">#3244</a>
            </td>
            <td>
                <b>
                    Bump go-kit/kit v0.9.0 to v0.10.0
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
- Update dependency go-kit/kit from v0.9.0 to v0.10.0

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->


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
        Created At 2022-02-22 00:22:23 +0000 UTC
    </div>
</div>

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

