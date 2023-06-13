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
                PR <a href="https://github.com/hyperledger/fabric/pull/4282" class=".btn">#4282</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.5 and Alpine to 3.18 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.5.
Bump Alpine images to 3.18 (Go 1.20.5 not available on Alpine 3.16).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 15:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4281" class=".btn">#4281</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.5 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.5.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 15:33:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4280" class=".btn">#4280</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.5.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 15:23:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4279" class=".btn">#4279</a>
            </td>
            <td>
                <b>
                    More verbose logs for etcdraft unit tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: Id6905e22f2826158150c8c36152dee1d9cf992dc

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

More verbose logs for etcdraft unit tests will make it easier to track down flakes

#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-13 13:26:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4278" class=".btn">#4278</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: select BFT or CFT orderer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Change-Id: I8661f23e7a8c5db6422a09a183b042088da6f0e5

#### Type of change
- New feature

#### Description
- When a channel is created in the peer, inspect the channel config, and according to the Orderer's consensus type, instantiate a CFT or BFT block puller.

- In addition, send the initial channel config and crypto provider to the deliverer, in preparation for it maintaining its own block verifier and connection source.

- Separate the "sleeper" to a different file and test it separately such that it can be a subcomponent in multiple implementations.

#### Related issues

Issue: #4277 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-12 13:40:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4276" class=".btn">#4276</a>
            </td>
            <td>
                <b>
                    fix typo in config bft
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Typo fix

#### Type of change

- Documentation update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-12 12:36:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4274" class=".btn">#4274</a>
            </td>
            <td>
                <b>
                    Update install scripts for v2.5.2
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

- Bug fix
- Documentation update

#### Description

Update install script and bootstrap script for v2.5.2.

#### Related issues



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
        Created At 2023-06-12 10:48:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4267" class=".btn">#4267</a>
            </td>
            <td>
                <b>
                    Restrict WAL usage to node.go (backport #4201)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4201 done by [Mergify](https://mergify.com).


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
        Created At 2023-06-07 15:11:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4266" class=".btn">#4266</a>
            </td>
            <td>
                <b>
                    Fix typo in logger name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                commmon -> common


#### Type of change

- Bug fix

#### Description

Typo in the word _common_ being written with 3 `m`'s instead of only 2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 06:30:06 +0000 UTC
    </div>
</div>

