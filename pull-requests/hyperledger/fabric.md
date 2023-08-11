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
                PR <a href="https://github.com/hyperledger/fabric/pull/4362" class=".btn">#4362</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.7 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.7.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 20:30:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4361" class=".btn">#4361</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.7 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.7.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 20:30:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4360" class=".btn">#4360</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.7.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 18:59:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4359" class=".btn">#4359</a>
            </td>
            <td>
                <b>
                    docs: fix link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a cherry-pick of this PR:
https://github.com/hyperledger/fabric-docs-i18n/pull/816

#### Type of change

- Documentation update

#### Description

There is a double paren when there should be a single paren, which breaks a link

#### Additional details

#### Related issues

#### Release Note

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 14:23:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4356" class=".btn">#4356</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc to 1.53.0 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note that grpc 1.52.0 changed behavior of Dial(),
empty string can no longer be passed.
Therefore this PR also updates tests that passed empty string.

Also remove the go.mod replace for github.com/cespare/xxhash/v2, it is no longer needed and the grpc update also updates github.com/cespare/xxhash/v2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-09 14:17:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4355" class=".btn">#4355</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc to 1.53.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note that grpc 1.52.0 changed behavior of Dial(),
empty string can no longer be passed.
Therefore this PR also updates tests that passed empty string.

Also remove the go.mod `replace` for github.com/cespare/xxhash/v2,
it is no longer needed and the grpc update also updates github.com/cespare/xxhash/v2.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-08 21:02:53 +0000 UTC
    </div>
</div>

