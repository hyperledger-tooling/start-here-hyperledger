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
                PR <a href="https://github.com/hyperledger/fabric/pull/4746" class=".btn">#4746</a>
            </td>
            <td>
                <b>
                    BFT chain unit tests: sync a node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

This PR aims to test whether a node can sync successfully when it's behind. 

#### Additional details

For the implementation, a synchronizer factory was needed.

#### Related issues

#4008
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 13:32:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4744" class=".btn">#4744</a>
            </td>
            <td>
                <b>
                    Update documentation on issue assignment process
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

- Documentation update

#### Description
This update clarifies the issue assignment process, addressing GitHub's permission limitations for general developers. It ensures the documentation accurately reflects how developers can engage with issues when direct self-assignment is not possible.

Addtionally, this patch includes other minor fixes in some documantations.
<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

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
        Created At 2024-03-11 02:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4743" class=".btn">#4743</a>
            </td>
            <td>
                <b>
                    Synchronizer dynamic block puller
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change


- Bug fix

#### Description

The simple synchronizer uses a static block puller which does not get updated.

#### Related issues
#4696 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-10 16:45:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4740" class=".btn">#4740</a>
            </td>
            <td>
                <b>
                    BFT synchronizer: expose timeouts to config
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

BFT synchronizer: expose timeouts to config

#### Related issues

#4719 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-10 11:57:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4739" class=".btn">#4739</a>
            </td>
            <td>
                <b>
                    Gossip test: Avoid warning in IDE
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

The current style of the code, of referencing the callback function directly from the slice
```
secondChannelServices[idx].callback
```
 generates a warning in the IDE.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-10 10:15:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4738" class=".btn">#4738</a>
            </td>
            <td>
                <b>
                    remove repetitive words
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

Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

remove repetitive words



#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

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
        Created At 2024-03-08 07:42:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4737" class=".btn">#4737</a>
            </td>
            <td>
                <b>
                    Bump github.com/onsi/ginkgo/v2 to v2.13.2 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/onsi/ginkgo/v2 to v2.13.2
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 07:40:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4736" class=".btn">#4736</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/protobuf to v1.33.0 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump google.golang.org/protobuf to v1.33.0.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 22:17:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4735" class=".btn">#4735</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.21.8
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 21:48:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4734" class=".btn">#4734</a>
            </td>
            <td>
                <b>
                    add embed files to the package chaincode (backport #4729)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4729 done by [Mergify](https://mergify.com).


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
        Created At 2024-03-07 21:41:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4733" class=".btn">#4733</a>
            </td>
            <td>
                <b>
                    change flag for ginkgo exec (backport #4728)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4728 done by [Mergify](https://mergify.com).


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
        Created At 2024-03-07 21:40:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4729" class=".btn">#4729</a>
            </td>
            <td>
                <b>
                    add embed files to the package chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recently [pr](https://github.com/hyperledger/fabric/pull/4726/checks) failed tests and failed to update the `google.golang.org/protobuf` package. 
The reason is that we added go:embed to the https://github.com/protocolbuffers/protobuf-go/blob/master/internal/editiondefaults/defaults.go. When building the package we didn't copy file editions_defaults.binpb and the build of the chaincode ended with an error.

After accepting this [pr](https://github.com/hyperledger/fabric/pull/4726/checks), you can update the package again 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 07:39:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4728" class=".btn">#4728</a>
            </td>
            <td>
                <b>
                    change flag for ginkgo exec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                --slow-spec-threshold is deprecated --slow-spec-threshold has been deprecated and will be removed in a future version of Ginkgo.  This feature has proved to be more noisy than useful.  You can use --poll-progress-after, instead, to get more actionable feedback about potentially slow specs and understand where they might be getting stuck.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 07:21:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4727" class=".btn">#4727</a>
            </td>
            <td>
                <b>
                    BFT: move shared peer & orderer block delivery client code to common
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

Move shared peer & orderer block delivery client code from `internal/pkg/peer` to `common/deliverclient`.
No functional change.

#### Related issues

#4350 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 18:38:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4726" class=".btn">#4726</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/protobuf to v1.33.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump google.golang.org/protobuf to v1.33.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 17:15:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4725" class=".btn">#4725</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.21.8.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 17:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4723" class=".btn">#4723</a>
            </td>
            <td>
                <b>
                    fix struct names in comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix struct names in comments
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 02:45:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4722" class=".btn">#4722</a>
            </td>
            <td>
                <b>
                    Nominate Tatsuya Sato as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tatsuya Sato has been contributing to Fabric for several years. In the last 6 months Tatsuya has increased contributions, becoming one of the most active contributors.

Tatsuya has contributed new chaincode lifecycle functions that required updating protos across Fabric repositories.
He has fixed issues with cert expiration warnings.

Beyond normal code contributions, Tatsuya has also been doing general  maintenance pull requests, for example maintaining the installation script, cleaning up Fabric docs,
and maintaining the fabric-samples repository.
He has also translated documentation into Japanese, and been active in pull request reviews.

Tatsuya has demonstrated knowledge and added value across a wide range of areas spanning new features and general maintenance. In short, Tatsuya has already been maintaining Fabric. I would welcome Tatsuya's help as an official maintainer.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 17:23:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4721" class=".btn">#4721</a>
            </td>
            <td>
                <b>
                    BFT SyncBuffer capacity
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

Allow the BFT synchronizer SyncBuffer capacity to be configured and increase min size to 100

#### Related issues

#4715 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 15:07:51 +0000 UTC
    </div>
</div>

