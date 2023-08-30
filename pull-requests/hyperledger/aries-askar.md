---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    Introduce uniffi module and Swift wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a replacement for the previous PR #110 using [uniffi](https://github.com/mozilla/uniffi-rs) to support Swift.
This uniffi module could be used for other languages such as Kotlin later.

As we have discussed in the Discord channel, holding many wrappers in one repo is not preferred, so I want to get some advice if there's a way to make this uniffi module a separate package that uses aries-askar as a dependency in another repo.
Any comment will be appreciated.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-25 06:33:19 +0000 UTC
    </div>
</div>

