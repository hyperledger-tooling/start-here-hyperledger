---
layout: default
title: hlf-operator
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/hlf-operator
---

# hlf-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Version 1.8.0-beta9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.8.0-beta9
                </span>
            </td>
            <td>
                ## Changelog
* 34e295d Fix CI/CD
* 7306ea2 Improve docs
* 1a33109 update docs
* 6c200d5 Fix kubectl plugin test
* 935454d Fix kubectl plugin test
* 2ffd160 Implement mainChannel update
* ec25f49 update secret key
* d386a6f update ci/cd
* 8408302 update test for channelcrd
* 2d27517 update README for new channelcrd
* 692f6e4 fix create follower channel
* a7052dd allow a CA or inline tls/sign cert for orderer organization
* 551c643 Filter by orderer nodes in the channels section. Add configurable channels in inspect.go
* b89a5e8 Remove required args flag
* bbadb1f Modify create.go mainchannel cmd
* 2bcda6f Update
* 3df2906 Add follower channel CLI
* b9800be Add follower channel CLI
* 224c8a8 Update go.mod
* 40c5c00 Upgrade to 1.17
* 5475f82 Fix pipelines
* 304cb61 Modify create.go
* f39d1d8 Upgrade k8s APIs Upgrade operator-lib Fix update-codegen.sh
* 4d1d57b add k8s clients for mainchannel and followerchannel
* 8f94a6e Wait for deployments to be ready
* 5f569fa Add livenessProbe and ReadinessProbe to chaincode deployment CRD
* 8fe1811 Fix add/remove organizations + typo on cAName -> caName
* ebe6c09 Fix pipelines
* abf49fa MVP of FabricFollowerChannel: - Add anchor peers - Join peers
* b26c425 MVP of FabricMainChannel, missing configure parameters
* b9e9927 register `FabricMainChannel` and `FabricFollowerChannel`
* cb2adb1 Upload CRDs
* f14d530 Update
* 3446c50 update docs
* 18ae883 Add inspect for organizations that don't have peers
* f41e2cc Default parameters externalchaincode
* f179152 Default resources when creating the CA
* 8b6df6f Safe defaults for signing
* 814e93c Set up affiliations per CA Set up signing parameters per CA
* d7e1ed0 remove unused krew-plugin.yaml (#107)
* fb03572 add new platforms for krew
* d6fb61b fix broken link
* 5db1eb6 fix enroll
* aee0f84 1.7.0 release (#95)
* 7d849c6 Use user defined peer capacity (#99)
* 94c3331 fix helm chart deployment template (#94)
* 5a29eb3 Update README.md (#92)
* c98bff2 Fix getting-started (Add command for cleaning up the chaincode). (#90)


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/hlf-operator/releases/tag/v1.8.0-beta9" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-20 10:02:13 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Version 1.8.0-beta10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.8.0-beta10
                </span>
            </td>
            <td>
                ## Changelog
* 8fe6962 Add AdminHosts to CSRHosts while creating the orderer node
* 39d04a7 Fix CI/CD
* 4ac76cf Improve docs
* 4475283 update docs
* ecc77bf Fix kubectl plugin test
* a2b4b28 Fix kubectl plugin test
* ccc0bcd Implement mainChannel update
* 920445e update secret key
* 40757fe update ci/cd
* dd3dbd9 update test for channelcrd
* 2d27517 update README for new channelcrd
* 692f6e4 fix create follower channel
* a7052dd allow a CA or inline tls/sign cert for orderer organization
* 551c643 Filter by orderer nodes in the channels section. Add configurable channels in inspect.go
* b89a5e8 Remove required args flag
* bbadb1f Modify create.go mainchannel cmd
* 2bcda6f Update
* 3df2906 Add follower channel CLI
* b9800be Add follower channel CLI
* 224c8a8 Update go.mod
* 40c5c00 Upgrade to 1.17
* 5475f82 Fix pipelines
* 304cb61 Modify create.go
* f39d1d8 Upgrade k8s APIs Upgrade operator-lib Fix update-codegen.sh
* 4d1d57b add k8s clients for mainchannel and followerchannel
* 8f94a6e Wait for deployments to be ready
* 5f569fa Add livenessProbe and ReadinessProbe to chaincode deployment CRD
* 8fe1811 Fix add/remove organizations + typo on cAName -> caName
* ebe6c09 Fix pipelines
* abf49fa MVP of FabricFollowerChannel: - Add anchor peers - Join peers
* b26c425 MVP of FabricMainChannel, missing configure parameters
* b9e9927 register `FabricMainChannel` and `FabricFollowerChannel`
* cb2adb1 Upload CRDs
* f14d530 Update
* 3446c50 update docs
* 18ae883 Add inspect for organizations that don't have peers
* f41e2cc Default parameters externalchaincode
* f179152 Default resources when creating the CA
* 8b6df6f Safe defaults for signing
* 814e93c Set up affiliations per CA Set up signing parameters per CA
* d7e1ed0 remove unused krew-plugin.yaml (#107)
* fb03572 add new platforms for krew
* d6fb61b fix broken link
* 5db1eb6 fix enroll
* aee0f84 1.7.0 release (#95)
* 7d849c6 Use user defined peer capacity (#99)
* 94c3331 fix helm chart deployment template (#94)
* 5a29eb3 Update README.md (#92)
* c98bff2 Fix getting-started (Add command for cleaning up the chaincode). (#90)


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/hlf-operator/releases/tag/v1.8.0-beta10" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-20 10:39:49 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Version 1.8.0-beta7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.8.0-beta7
                </span>
            </td>
            <td>
                ## Changelog
* 212241b Fix kubectl plugin test
* 38394f3 Fix kubectl plugin test
* 0dce830 Implement mainChannel update
* 626aa55 update secret key
* 0c20c36 update ci/cd
* 205c88f update test for channelcrd
* 41fbc88 update README for new channelcrd
* 692f6e4 fix create follower channel
* a7052dd allow a CA or inline tls/sign cert for orderer organization
* 551c643 Filter by orderer nodes in the channels section. Add configurable channels in inspect.go
* b89a5e8 Remove required args flag
* bbadb1f Modify create.go mainchannel cmd
* 2bcda6f Update
* 3df2906 Add follower channel CLI
* b9800be Add follower channel CLI
* 224c8a8 Update go.mod
* 40c5c00 Upgrade to 1.17
* 5475f82 Fix pipelines
* 304cb61 Modify create.go
* f39d1d8 Upgrade k8s APIs Upgrade operator-lib Fix update-codegen.sh
* 4d1d57b add k8s clients for mainchannel and followerchannel
* 8f94a6e Wait for deployments to be ready
* 5f569fa Add livenessProbe and ReadinessProbe to chaincode deployment CRD
* 8fe1811 Fix add/remove organizations + typo on cAName -> caName
* ebe6c09 Fix pipelines
* abf49fa MVP of FabricFollowerChannel: - Add anchor peers - Join peers
* b26c425 MVP of FabricMainChannel, missing configure parameters
* b9e9927 register `FabricMainChannel` and `FabricFollowerChannel`
* cb2adb1 Upload CRDs
* f14d530 Update
* 3446c50 update docs
* 18ae883 Add inspect for organizations that don't have peers
* f41e2cc Default parameters externalchaincode
* f179152 Default resources when creating the CA
* 8b6df6f Safe defaults for signing
* 814e93c Set up affiliations per CA Set up signing parameters per CA
* d7e1ed0 remove unused krew-plugin.yaml (#107)
* fb03572 add new platforms for krew
* d6fb61b fix broken link
* 5db1eb6 fix enroll
* aee0f84 1.7.0 release (#95)
* 7d849c6 Use user defined peer capacity (#99)
* 94c3331 fix helm chart deployment template (#94)
* 5a29eb3 Update README.md (#92)
* c98bff2 Fix getting-started (Add command for cleaning up the chaincode). (#90)


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/hlf-operator/releases/tag/v1.8.0-beta7" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-18 07:40:46 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Version 1.8.0-beta6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.8.0-beta6
                </span>
            </td>
            <td>
                ## Changelog
* e3c8029 Implement mainChannel update
* 0a5cf85 update secret key
* b52d5d8 update ci/cd
* 4559719 update test for channelcrd
* 2c3fa20 update README for new channelcrd


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/hlf-operator/releases/tag/v1.8.0-beta6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-09-17 11:02:05 +0000 UTC
    </span>
</div>

