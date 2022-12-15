---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    [Documentation update]Update configtx.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix following issue after run `configtxgen -profile OrgsOrdererGenesis -outputBlock /tmp/hyperledger/org0/orderer/genesis.block -channelID syschannel` by fix format.
* 'Organizations[0]' has invalid keys: OrdererEndpoints
* 'Profiles[TwoOrgsOrdererGenesis].Orderer.Organizations[0]' has invalid keys: OrdererEndpoints
* Profiles[TwoOrgsOrdererGenesis].Orderer.Organizations[0]' has invalid keys: OrdererEndpoints [recovered]
* 'Profiles[TwoOrgsOrdererGenesis].Orderer.Organizations[0]' has invalid keys: OrdererEndpoints
* Error reading configuration: While parsing config: yaml: line 85: mapping values are not allowed in this context
* '' has invalid keys: orgschannel, orgsorderergenesis
* 'Profiles[OrgsOrdererGenesis].Consortiums[Organizations]' expected a map, got 'slice'

Signed-off-by: LF <xiayanzheng@outlook.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

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
        Created At 2022-12-15 15:29:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    [Bug fix]Update docker_compose.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: LF <xiayanzheng@outlook.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

<!--- Describe your changes in detail, including motivation. -->
Add tabs before every service, fix `ERROR: In the file './docker-compose.yaml', service must be a mapping, not a NoneType`. after running the `docker-compose up ca-tls` command.


#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
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
        Created At 2022-12-11 12:03:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    Publish release artifacts to conventional installation paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Bug fix

#### Description

This PR publishes the v1.5.6-beta release artifacts to GH as artifacts, stripping the semrev 'v' character for alignment with the traditional install-fabric.sh scripts. 

#### Additional details

#### Related issues

#### Release Note

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 18:37:45 +0000 UTC
    </div>
</div>

