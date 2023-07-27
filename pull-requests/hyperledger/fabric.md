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
                PR <a href="https://github.com/hyperledger/fabric/pull/4334" class=".btn">#4334</a>
            </td>
            <td>
                <b>
                    Address Docs Dependency Vulnerability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)
- Documentation update

#### Description

Updates the version of Sphinx used to generate the Fabric Documentation to v7.1 from v1.8.2, which was released many years ago.  

#### Additional details

Along the way, it addresses two security vulnerabilities that have been discovered for Pygments. I tested it by running `make docs` in my local clone of the fabric repo and then checking the resultant output using Chrome on my Mac laptop.  It looked identical to https://hyperledger-fabric.readthedocs.io/

#### Related issues

As per https://github.com/hyperledger/fabric/issues/4333.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 18:09:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4330" class=".btn">#4330</a>
            </td>
            <td>
                <b>
                    Remove ReplicationBackgroundRefrshInterval
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's not used anymore.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 13:48:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4328" class=".btn">#4328</a>
            </td>
            <td>
                <b>
                    fix: missing tag for make docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Fix missing tag for `make docker`
#### Type of change

- Bug fix

#### Description

When `make docker` make file is miss the tag. So, `make docker-tag-latest` and `make docker-tag-stable` will not work

#### Additional details

Reproduce: run `make docker-tag-latest` or `make docker-tag-stable` after run `make docker`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 14:24:34 +0000 UTC
    </div>
</div>

