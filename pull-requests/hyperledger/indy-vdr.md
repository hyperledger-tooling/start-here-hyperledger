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
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    ci: fix lerna version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To address #217, I've pinned lerna to the latest version and run a `lerna repair` (as suggested in [Lerna 7.0.0 release notes](https://github.com/lerna/lerna/releases/tag/7.0.0)) to remove wrong configurations.

If this approach is OK, I think we'll need to do the same for aries-askar (already updated to lerna 7.x but config files not fixed yet) and maybe anoncreds-rs (currently using lerna 6.x).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 17:27:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    fix(js): add missing parameters to rn wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update cbindgen config and README to work with current repo status (which includes workspaces)
- Update existing React Native binding methods according to current FFI layer. By this I mean "not to crash" and work with the same features as before

Both NodeJS and React Native wrappers will still need to be updated to include all functions introduced for did:indy support (like the ones from resolver crate). 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 15:05:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    Update versions to 0.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-11 22:42:49 +0000 UTC
    </div>
</div>

