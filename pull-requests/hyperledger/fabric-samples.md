---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/650" class=".btn">#650</a>
            </td>
            <td>
                <b>
                    Add external chaincode service for Nano Test Network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This addresses Issue #504. This sample offers an option to run
a fabric network without using any containers at all. Used along
with the Nano Test Network, everything is run natively on the host
machine.

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 15:35:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/649" class=".btn">#649</a>
            </td>
            <td>
                <b>
                    fix docker compose version 2 -> 2.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Earlier compose version was giving a property error when running the [fabric-samples/test-network/network.sh](https://github.com/hyperledger/fabric-samples/blob/main/test-network/network.sh) script.
![compose_error](https://user-images.githubusercontent.com/16841301/154474662-ceb92110-ba54-4887-935d-bc0db32da006.png)

Docker Compose Documentation says that the property [networks:name](https://docs.docker.com/compose/compose-file/compose-file-v2/#name-1) was added in [v2.1](https://docs.docker.com/compose/compose-file/compose-versioning/#version-21) file format.
Signed-off-by: kaushikkumarbora <kaushikkumarbora@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 11:47:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/647" class=".btn">#647</a>
            </td>
            <td>
                <b>
                    Improve REST sample README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add that one needs to have the ledger initialized for the sample to
work.

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 10:49:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/646" class=".btn">#646</a>
            </td>
            <td>
                <b>
                    Kieran test
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
        Created At 2022-02-15 17:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/645" class=".btn">#645</a>
            </td>
            <td>
                <b>
                    Fix sample external chaincode Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Podman isn't as lenient as docker when it comes to the syntax of the
Dockerfile and insists on getting the ARG command properly scoped.
This fixes this error:
...
[2/2] STEP 12/15: EXPOSE $CC_SERVER_PORT
Error: error building at STEP "EXPOSE $CC_SERVER_PORT": EXPOSE requires at least one argument

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 14:34:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/643" class=".btn">#643</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.7 to 1.14.8 in /asset-transfer-basic/rest-api-typescript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.7 to 1.14.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/3d81dc3237b4ffe8b722bb3d1c70a7866657166e"><code>3d81dc3</code></a> Release version 1.14.8 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/62e546a99c07c3ee5e4e0718c84a6ca127c5c445"><code>62e546a</code></a> Drop confidential headers across schemes.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.7...v1.14.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.7&new-version=1.14.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-samples/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 02:38:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/641" class=".btn">#641</a>
            </td>
            <td>
                <b>
                    Issue 602
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Flow:

Check if docker network is running. 
If network is not running exit
If running, and containers are present + certs are present skip network up
If running, containers are not present then we should networkUp
If containers exist but certs don’t, bring network down and then networkUp

When containers are running but for some reason peerOrganisation dir was not present, the following error: 
`Failed to generate channel configuration transaction...` may be awkward to debug. So this is why there is a check to see if peerOrg does not exist but the containers do. 


Test Cases: 

1) Docker is not running 
```
./network.sh up createChannel -ca
Using docker and docker-compose
Creating channel 'mychannel'.
If network is not up, starting nodes with CLI timeout of '5' tries and CLI delay of '3' seconds and using database 'leveldb 
docker network is required to be running to create a channel
```

2) Docker is running but containers are not, peerOrganizations directory exists
```
./network.sh up createChannel -ca
Using docker and docker-compose
Creating channel 'mychannel'.
If network is not up, starting nodes with CLI timeout of '5' tries and CLI delay of '3' seconds and using database 'leveldb 
Bringing up network
LOCAL_VERSION=2.4.1
DOCKER_IMAGE_VERSION=2.4.1
CA_LOCAL_VERSION=1.5.2
CA_DOCKER_IMAGE_VERSION=1.5.2
WARN[0000] Found orphan containers ([ca_org2 ca_org1 ca_orderer]) for this project. If you removed or renamed this service in your compose file, you can run this command with the --remove-orphans flag to clean it up. 
[+] Running 4/4
 ⠿ Container peer0.org2.example.com  Started                                                                                                                                                                                                                               0.6s
 ⠿ Container peer0.org1.example.com  Started                                                                                                                                                                                                                               0.6s
 ⠿ Container orderer.example.com     Started                                                                                                                                                                                                                               0.6s
 ⠿ Container cli                     Started  
```
3) Containers running but  peerOrganizations directory does not exist
```
./network.sh up createChannel -ca
Using docker and docker-compose
Creating channel 'mychannel'.
If network is not up, starting nodes with CLI timeout of '5' tries and CLI delay of '3' seconds and using database 'leveldb with crypto from 'Certificate Authorities'
Decomposing compose-test-net.yaml
[+] Running 10/7
 ⠿ Container orderer.example.com          Removed                                                                                                                                                                                                                          0.2s
 ⠿ Container cli                          Removed                                                                                                                                                                                                                         10.2s
 ⠿ Container peer0.org1.example.com       Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container peer0.org2.example.com       Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container ca_orderer                   Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container ca_org2                      Removed                                                                                                                                                                                                                          0.3s
 ⠿ Container ca_org1                      Removed                                                                                                                                                                                                                          0.3s
 ⠿ Volume compose_peer0.org2.example.com  Removed                                                                                                                                                                                                                          0.0s
 ⠿ Volume compose_peer0.org1.example.com  Removed                                                                                                                                                                                                                          0.0s
 ⠿ Volume compose_orderer.example.com     Removed                                                                                                                                                                                                                          0.0s
Decomposing compose-couch.yaml
service "peer0.org1.example.com" has neither an image nor a build context specified: invalid compose project
Decomposing compose-ca.yaml
[+] Running 1/0
 ⠿ compose  Warning: No resource found to remove                                                                                                                                                                                                                           0.0s
Error: No such volume: docker_orderer.example.com
Error: No such volume: docker_peer0.org1.example.com
Error: No such volume: docker_peer0.org2.example.com
Removing remaining containers
Removing generated chaincode docker images
"docker kill" requires at least 1 argument.
See 'docker kill --help'.

Usage:  docker kill [OPTIONS] CONTAINER [CONTAINER...]

Kill one or more running containers
Bringing up network
LOCAL_VERSION=2.4.1
DOCKER_IMAGE_VERSION=2.4.1
CA_LOCAL_VERSION=1.5.2
...
```

Signed-off-by: Kieran O Mahony [Kieran.O.Mahony1@ibm.com](mailto:Kieran.O.Mahony1@ibm.com)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 23:28:48 +0000 UTC
    </div>
</div>

