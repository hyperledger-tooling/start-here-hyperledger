---
layout: default
title: sawtooth-sdk-rust
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-rust
---

# sawtooth-sdk-rust <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-rust){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-rust/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    WIP: Break out features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hello,

I've created this PR to get comments on my strategy for this solution. If this is satisfactory, I'll clean everything up.

I'm working on a project targeting wasm in the browser (via wasm-pack / wasm-bindgen). For this use case, I obviously can't have any of the ZMQ code being included. I also don't particularly need the signing code (I am using cylinder instead).

The main idea is to keep the default behavior as it functioned previously, but also to allow bringing in the SDK using whatever subset of the features you need.

Thanks in advance for any feedback.

Sincerely,
Bill
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-22 02:14:55 +0000 UTC
    </div>
</div>

