---
layout: default
title: fabric-amcl
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-amcl
---

# fabric-amcl <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-amcl){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-amcl/pull/22" class=".btn">#22</a>
            </td>
            <td>
                <b>
                    Correct build tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The previous patch used

```
//go:build amd64 || arm64
```

as build tag for 64-bit architectures. However this was unvoluntarily discarding other 64-bit platforms (such as `wasm`) that were previously supported. The issue has been fixed by replacing the tag with

```
//go:build !386 && !arm
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 17:36:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-amcl/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    32bit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for 32-bit platforms (and also pulls the latest sources from miracl/core)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 14:49:03 +0000 UTC
    </div>
</div>

