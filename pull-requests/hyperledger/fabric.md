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
                PR <a href="https://github.com/hyperledger/fabric/pull/4680" class=".btn">#4680</a>
            </td>
            <td>
                <b>
                    up consensus library
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
        Created At 2024-02-15 05:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4679" class=".btn">#4679</a>
            </td>
            <td>
                <b>
                    BFT chain unit tests: create a new chain without errors
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

The purpose of this PR is to create BFT chain unit tests. 
The first step is to create an active chain using mocks. 

#### Related issues

issue #4008 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 15:35:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4678" class=".btn">#4678</a>
            </td>
            <td>
                <b>
                    Switch to bccsp, metrics, flogging in fabric-lib-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following packages are being moved from fabric to fabric-lib-go so that they can be shared across fabric and fabric-ca:

- github.com/hyperledger/fabric/bccsp
- github.com/hyperledger/fabric/common/flogging
- github.com/hyperledger/fabric/common/metrics (including the gendoc utility)

The [PR](https://github.com/hyperledger/fabric-ca/pull/404) over in fabric-ca finally removes the fabric-ca dependency on core fabric.

This commit updates fabric to use the common code in fabric-lib-go.

For now a temporary branch in fabric-lib-go is used, see the corresponding [commit](https://github.com/hyperledger/fabric-lib-go/commit/cdae4d4a292dbad122b93a2c5c70bc61d846e990).
After this PR is reviewed and merged fabric-lib-go will be released and the dependency here will be updated to a real versioned release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 02:52:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4674" class=".btn">#4674</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/tools from v0.14.0 to v0.17.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump golang.org/x/tools to v0.17.0.

Note that gendoc broke with v0.15.0 with error:
panic: can't determine type sizes for compiler "" on GOARCH ""

It turns out that gendoc didn't need the problematic `packages.NeedTypesInfo` and therefore this option is now removed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 20:40:17 +0000 UTC
    </div>
</div>

