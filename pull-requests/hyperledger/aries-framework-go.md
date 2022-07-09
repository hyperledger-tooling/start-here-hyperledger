---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3270" class=".btn">#3270</a>
            </td>
            <td>
                <b>
                    feat: add ext db packages to REST Agent (#3269)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ana Maria Franco <afrancoc2000@gmail.com>

**Title:**
Adding extended database packages to the Rest Agent

**Description:**
The Rest Agent doesn't have an easy way to use the [extended package databases](https://github.com/hyperledger/aries-framework-go-ext/tree/ce8776c10037404f5c31a67aced0df6828bc4c28), so, I'm adding the posibility to use them in here.

[Issue 3269](https://github.com/hyperledger/aries-framework-go/issues/3269)

**Summary:**

I'm adding support for the Rest Agent to: couchdb, mongodb, mysql, postgresql, from the [aries-framework-go-ext](https://github.com/hyperledger/aries-framework-go-ext) package, and updating the docs.

Also I ran `go mod tidy -go=1.16 && go mod tidy -go=1.17` and updated the go.mod keeping compatibility with go 1.16. Not sure if compatibility with go 1.16 is still wanted.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-09 14:28:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3268" class=".btn">#3268</a>
            </td>
            <td>
                <b>
                    feat: Legacy Anoncrypt(RFC-0019) DIDComm v1 implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Legacy Anoncrypt(RFC-0019) DIDComm v1 implementation


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 14:06:56 +0000 UTC
    </div>
</div>

