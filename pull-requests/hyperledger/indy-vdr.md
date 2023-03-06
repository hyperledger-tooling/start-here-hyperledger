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
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/170" class=".btn">#170</a>
            </td>
            <td>
                <b>
                    fix(js): several fixes for js wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Similar to https://github.com/hyperledger/aries-askar/pull/111, but for indy-vdr
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 13:44:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    re-use existing indy-node-container builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - simplifies the docker image for the local pool
- adds a small bash script that can be re-used for different tests and local testing

Successor of #112
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 07:13:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Build updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update the base images used in `cross` builds
- Verify that Python wheels (and by extension npm modules) are compatible with manylinux 2014
- Only use build.sh (now build-universal.sh) for MacOS universal builds, otherwise prefer `cargo build`
- Improve caching of Rust dependencies
- Minor adjustments to build-xcframework script
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 00:31:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    quick fix for ffi bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Re-generated the header file and adjusted the typescript calls for attrib/nym with the new parameters. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 23:12:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    Merge did:indy support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently, tests are failing with the JS wrapper due to a timeout in GetAttribRequest. I think this might be a compatibility issue with the did:indy-supporting indy-node version, but I'm not certain.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 17:28:34 +0000 UTC
    </div>
</div>

