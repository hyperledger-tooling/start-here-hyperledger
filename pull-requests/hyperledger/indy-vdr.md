---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/116" class=".btn">#116</a>
            </td>
            <td>
                <b>
                    updated ZMQ to the latest version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - No more zmq vendored feature
- makes cross-compilation a lot easier as `libzmq3-dev` is not required anymore (this is required for the upcoming Android pipeline)
- Tests still pass 
- [changelog](https://github.com/erickt/rust-zmq/releases/tag/v0.10.0) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 19:54:22 +0000 UTC
    </div>
</div>

