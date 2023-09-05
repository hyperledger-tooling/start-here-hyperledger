---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Support for Hyperledger Fabric 2.5 with new features and enhancements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v2.0.0
                </span>
            </td>
            <td>
                <!-- (SPDX-License-Identifier: CC-BY-4.0) -->  <!-- Ensure there is a newline before, and after, this line -->


## New Features

* Health status of peers
    - BE-340 Display health status of peers and orderers - FrontEnd (#342)
    - BE-331 Display health status of peers and orderers- Backend (#337)
* Search by block number, txn id, blockrange
    - Add Frontend blocks view pagination and block range search (#371)
    - Added search functonality to dashboard so user can search with Txn hash/Block no from there itself (#357)
    - BE 334 fetch data by block number, block range and transaction id - Backend (#338)
* Display chaincode metadata
    - chaincode metadata changes added (#383)
    - Frontend- Display chaincode metadata in chaincodes tab (#368)
* Move container images from dockerhub to ghcr
    - move to ghcr registry (#382)
* Migrate CI to github actions
    - added github ci (#339)


## Bug Fixes and Updates

* updated docker-compose files with ghcr images (#438)
* updated node version in ci files (#437)
* BE-433 | Fix package related breaking issues (#434)
* BE431 | Fix-Test-case Failing (#432)
* Release v2.0.0 (#430)
* BE-422 | UI Responsiveness and Misc (#427)
* update swagger.json (#424)
* BE-420 | Ledger Height and Peers Status is not updating w.r.t multiple channels (#421)
* Integrate SonarCloud (#419)
* BE-417 | resolve sigint bad trap and unexpected error (#418)
* BE-415 | remove duplicate peerStatus api call (#416)
* BE-406 | send channelhash to metadata api (#412)
* Backend- Improper updation of Txn Count and Chaincodes list (#411)
* Display correct chaincode metadata fix in the backend (#410)
* Blocks pagination query fix in the backend (#407)
* BE-399 | Show transaction details for the first Config type transaction (#403)
* fix incorrect default password on README.md (#402)
* bugFixes for the release (#398)
* updates for dashboard UI responsiveness for cards and pie chart (#391)
* Updated run_e2e_test.sh (#380)
* Backend - Pagination implementation for Blocks Tab (#378)
* Chaincode count on Dashboard is incorrect (#377)
* Add validations to search functionality blockId and blockRange (#376)
* Empty org is being displayed while fetching the list of orgs (#374)
* Update Dockerfile (#370)
* Update MAINTAINERS.md (#366)
* maintainers contact (#363)
* BE-346-Added Pagination for Transaction view - Backend (#351)
* added pagination for transactions view frontend (#350)
* fix failing unit test cases (#349)
* BE-340 Display health status of peers and orderers - FrontEnd (#342)
* update CODEOWNERS (#330)
* added github issue form (#325)
* Disable Sonar cloud on PRs

## Known Vulnerabilities


package-lock.json
```

ejs  <3.1.7
Severity: critical
ejs template injection vulnerability - https://github.com/advisories/GHSA-phwq-j96m-2c2q
fix available via `npm audit fix --force`

```
client/package-lock.json
```

ejs  <3.1.7
Severity: critical
ejs template injection vulnerability - https://github.com/advisories/GHSA-phwq-j96m-2c2q
fix available via `npm audit fix --force`

flat  <5.0.1
Severity: critical
flat vulnerable to Prototype Pollution - https://github.com/advisories/GHSA-2j2x-2gpw-g8fm
fix available via `npm audit fix --force`

immer  <=9.0.5
Severity: critical
Prototype Pollution in immer - https://github.com/advisories/GHSA-c36v-fmgq-m8hx
Prototype Pollution in immer - https://github.com/advisories/GHSA-33f9-j839-rf8h
fix available via `npm audit fix`

loader-utils  2.0.0 - 2.0.3
Severity: critical
loader-utils is vulnerable to Regular Expression Denial of Service (ReDoS) via url variable - https://github.com/advisories/GHSA-3rfm-jhwj-7488
loader-utils is vulnerable to Regular Expression Denial of Service (ReDoS) - https://github.com/advisories/GHSA-hhq3-ff78-jv3g
Prototype pollution in webpack loader-utils - https://github.com/advisories/GHSA-76p3-8jx3-jpfq
fix available via `npm audit fix`

shell-quote  <=1.7.2
Severity: critical
Improper Neutralization of Special Elements used in a Command in Shell-quote - https://github.com/advisories/GHSA-g4rg-993r-mgx7
fix available via `npm audit fix`

```
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/blockchain-explorer/releases/tag/v2.0.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-05 14:36:25 +0000 UTC
    </span>
</div>

