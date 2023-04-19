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
                PR <a href="https://github.com/hyperledger/fabric/pull/4175" class=".btn">#4175</a>
            </td>
            <td>
                <b>
                    Revert "Fix firewall warnings for integration tests on Mac"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 412f3661cb05061a0a9413d16b24f5326f07b3fa.

The change caused integration tests to fail on a number of developer macs (both amd64 and arm64).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 14:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4174" class=".btn">#4174</a>
            </td>
            <td>
                <b>
                    Update dependencies (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update dependencies to match the known good levels in release-2.5. This will simplify maintenance and support between the two LTS releases and resolve vulnerability issues in these dependencies.

- github.com/docker/docker
- github.com/opencontainers/runc
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 14:16:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4173" class=".btn">#4173</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove sys chan from registrar
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

Remove the system channel from the multichannel.Registrar

#### Related issues

#3515 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 14:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4171" class=".btn">#4171</a>
            </td>
            <td>
                <b>
                    Update dependencies (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update dependencies to match the known good levels in release-2.5. This will simplify maintenance and support between the two LTS releases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 03:07:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4170" class=".btn">#4170</a>
            </td>
            <td>
                <b>
                    chore(ci): move to dedicated Fabric runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This moves Fabric from a cluster of runners to a dedicated Fabric set

#### Type of change

- CI
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 00:42:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4168" class=".btn">#4168</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.3 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.3.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 14:42:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4167" class=".btn">#4167</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.3 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.3.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 14:25:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4166" class=".btn">#4166</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.3.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 14:20:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4165" class=".btn">#4165</a>
            </td>
            <td>
                <b>
                    Orderer v3: prevent join to system channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                


Change-Id: I8a8a0d8810bf8337b66c07434d3a6d392ca963f4

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Prevent a system channel block from being accepted as valid input to channel participation join.

#### Related issues

Issue: #3515 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 14:20:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4164" class=".btn">#4164</a>
            </td>
            <td>
                <b>
                    Fix cert sanitation with go v1.19 (backport #3774 release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                -Update to go v1.19.
-Fix cert sanitation to work on Go 1.19 (Backport https://github.com/hyperledger/fabric/pull/3774 to release-2.2)
-Fix idemix revocation_test to work on Go 1.19
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 16:19:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4161" class=".btn">#4161</a>
            </td>
            <td>
                <b>
                    chore(ci): try new builers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 14:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4159" class=".btn">#4159</a>
            </td>
            <td>
                <b>
                    Fix failure in 'basic checks'
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

This patch fixes failure during 'basic checks' in the CI. It is possibly caused by the update of Go to v1.20.

#### Additional details

During the "basic checks" job, the command references are compared with the generated ones. Since the Go version is updated to v1.20, the CI job generates slightly different documents from those in the repository, which were generated with the previous versions of Go.

#### Related issues

#4157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 09:47:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4158" class=".btn">#4158</a>
            </td>
            <td>
                <b>
                    Fix typo regarding current LTS release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Fix typo regarding the current LTS release in README
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 09:39:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4157" class=".btn">#4157</a>
            </td>
            <td>
                <b>
                    Add docs for 'ledgerutil verify'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

This is a backport of #4098 to release-2.5, fixing the failed automated backport #4153.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 05:27:01 +0000 UTC
    </div>
</div>

