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
                PR <a href="https://github.com/hyperledger/fabric/pull/3544" class=".btn">#3544</a>
            </td>
            <td>
                <b>
                    change params exec ginkgo v2
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
        Created At 2022-07-25 19:37:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3542" class=".btn">#3542</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove kafka from viperutil
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

Remove kafka from viperutil

#### Related issues

Epic: #3511 
Issue: #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 13:57:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3541" class=".btn">#3541</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove Kafka from localconfig
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

Remove Kafka from orderer/localconfig package and orderer.yaml

#### Related issues

Epic: #3511 
Issue: #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 12:43:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3539" class=".btn">#3539</a>
            </td>
            <td>
                <b>
                    V2.5 Capabilities For Purge Private Data
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

<!--- Describe your changes in detail, including motivation. -->

- New application and channel capabilities version for v2.5 release to allow for the purge private data operation

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

- #3029 

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
        Created At 2022-07-22 13:46:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3538" class=".btn">#3538</a>
            </td>
            <td>
                <b>
                    Orderer V3: Kafka orderer cleanup
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

Clean the orderer package from kafka references.

#### Related issues

Epic: #3511 
Issue: #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 14:26:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3537" class=".btn">#3537</a>
            </td>
            <td>
                <b>
                    Orderer V3: Kafka cleanup - msgprocessor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I0202428c2b5dc571460474efc6d60dbc4fc60273


#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Clean kafka references in the msgprocessor maintenancefilter.

#### Related issues

Epic: #3511 
Issue: #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 13:59:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3536" class=".btn">#3536</a>
            </td>
            <td>
                <b>
                    Unfreeze active nodes metrics once a consenter is evicted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixed active nodes metrics for etcdraft when a node is evicted. Instead of being frozen we set it to 0 once halt is called. Tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 12:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3535" class=".btn">#3535</a>
            </td>
            <td>
                <b>
                    ExternalBuilder PropagateEnvironment fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While I was working on #3534 I realized that the master branch has also a potential issue with PropagateEnvorinment field.
A different implementation/version of the unmarshaller might set `builder.PropagateEnvironment` to nil or empty slice. In the last case PropagateEnvironment won't have a correct value. The fix is to use a bulletproof check `builder.PropagateEnvironment == nil` => `len(builder.PropagateEnvironment) == 0`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 23:47:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3534" class=".btn">#3534</a>
            </td>
            <td>
                <b>
                    [Release-2.2 BP FAB-2643]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a backport of pull request https://github.com/hyperledger/fabric/pull/2643

Because we can't upgrade viper to `v1.1.1` in which the bug of shadowing a key is fixed and hooks are introduced, I had to find a workaround to simplify the backport as more as possible. 

Also, I added a test and a short explanation for overriding the list of system chaincodes. The default approach with env var `CORE_CHAINCODE_SYSTEM_XXX: enabled` won't work due to a bug in viper in earlier versions. I agree that bumping it to v1.1.1 requires too many changes and might break the LTS release. 

updated a few related tests to use strings as viper config values instead of variables.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 14:03:47 +0000 UTC
    </div>
</div>

