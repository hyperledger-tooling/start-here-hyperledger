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
                PR <a href="https://github.com/hyperledger/fabric/pull/4444" class=".btn">#4444</a>
            </td>
            <td>
                <b>
                    Use golang 1.21.1 to fix vulnerabilities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I62c42a07bc4577e4c734a674878f0fe11a517edf

This patchset upgrade Go version from Go 1.20.7 to 1.21.1.

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

There are two vulnerabilities in Go 1.20: GO-2023-2041 and GO-2023-2043,
      which exist in package html/template and are used in
      core/middleware.

The vulnerabilities are fixed in Go 1.21.1.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 05:15:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4441" class=".btn">#4441</a>
            </td>
            <td>
                <b>
                    fix network diagrams R4 error (#4436)
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

I've fixed 4 diagrams on network page in documentation based on @satota2's suggestion.

Resolves #4436.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 16:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4440" class=".btn">#4440</a>
            </td>
            <td>
                <b>
                    smart BFT GRPC leader sends proposal to follower test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                SmartBFT integration test:
The leader is using GRPC to send a proposal to the follower, checking that the signature validation is correct.

#### Type of change

- Test update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 12:19:19 +0000 UTC
    </div>
</div>

