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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Cleanup maintainers list
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
        Created At 2022-04-08 19:39:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Release commit for v1.5.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release commit for v1.5.3.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 21:20:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    test: use `T.TempDir` to create temporary test directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

A testing cleanup. 

This pull request replaces `ioutil.TempDir` with `t.TempDir`. We can use the `T.TempDir` function from the `testing` package to create temporary directory. The directory created by `T.TempDir` is automatically removed when the test and all its subtests complete. 

Reference: https://pkg.go.dev/testing#T.TempDir

#### Additional details

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 15:22:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Undo breaking changes to exported packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Relocation of these packages should only have been done along with a major version change to the module.

https://go.dev/doc/modules/version-numbers

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 16:17:34 +0000 UTC
    </div>
</div>

