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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/344" class=".btn">#344</a>
            </td>
            <td>
                <b>
                    Adds v1.5.6-beta2 release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Release Note

v1.5.6-beta2 Release Notes - Dec 15, 2022
===================================

v1.5.6-beta2 is a beta release, providing updates for the following issues in the Fabric CA:

- Builds native arm64 CA binaries for linux and darwin
- Builds multi-platform CA docker images for arm64 and amd64 with `buildx`
- Adds debug information for a mysterious [idemix error message](https://github.com/hyperledger/fabric-ca/pull/339)


Dependencies
------------

Fabric CA v1.5.6 has been tested with the following dependencies:
- Go 1.18.8
- Alpine 3.17 (for Docker images)

Changes, Known Issues, and Workarounds
--------------------------------------

None.

Known Vulnerabilities
---------------------
- FABC-174 Commands can be manipulated to delete identities or affiliations

  This vulnerability can be resolved in one of two ways:

    1) Use HTTPS (TLS) so that the authorization header is not in clear text.

    2) The token generation/authentication mechanism was improved to optionally prevent
       token reuse. As of v1.4 a more secure token can be used by setting environment variable:

  FABRIC_CA_SERVER_COMPATIBILITY_MODE_V1_3=false

  However, it cannot be set to false until all clients have
  been updated to generate the more secure token and tolerate
  FABRIC_CA_SERVER_COMPATIBILITY_MODE_V1_3=false.
  The Fabric CA client has been updated in v1.4 to generate the more secure token.
  The Fabric SDKs will be updated by v2.0 timeframe to generate the more secure token,
  at which time the default for Fabric CA server will change to:
  FABRIC_CA_SERVER_COMPATIBILITY_MODE_V1_3=false

Resolved Vulnerabilities
------------------------
None.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 20:22:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/343" class=".btn">#343</a>
            </td>
            <td>
                <b>
                    Publishes release images to the docker.io, not ghcr.io container registry.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- CI pipeline

#### Description

This PR changes the target container registry from ghcr.io to docker.io. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 18:41:03 +0000 UTC
    </div>
</div>

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

