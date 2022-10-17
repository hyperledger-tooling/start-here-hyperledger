---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1978" class=".btn">#1978</a>
            </td>
            <td>
                <b>
                    chore: fix ACAPY_PROMOTE-AUTHOR-DID flag 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                using underscore instead of hyphen

closes #1965 

Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 13:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1977" class=".btn">#1977</a>
            </td>
            <td>
                <b>
                    fix: public did mediator routing keys as did keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes an issue @reflectivedevelopment found while using the recent changes made to support routing keys associated with public DID endpoints.

Without this fix, when creating a public DID OOB invitation, creation will fail due to no DIDComm service being found. This stemmed from PyDID expecting that routing keys be expressed strictly as DID URLs. Previously, we were resolving the routing keys as raw base58 encoded public keys. This PR makes it so that routing keys are resolved as did:key url values (if already did:key, simply pass through the values but if not, transform into did:key urls).

Credit to @cjhowland for doing most of the digging on this issue :slightly_smiling_face: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 18:52:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1975" class=".btn">#1975</a>
            </td>
            <td>
                <b>
                    Author demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Self-contained demo showing how to start up an author agent to to connect to an endorser service

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 17:25:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1973" class=".btn">#1973</a>
            </td>
            <td>
                <b>
                    Fix: web.py dependency - integration tests & demos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 00:13:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1970" class=".btn">#1970</a>
            </td>
            <td>
                <b>
                    Fix: `--mediator-invitation` with OOB invitation + cleanup 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>

The following issues were found as part of loadgenerator test setup.
- `--mediator-invitation` was failing with OOB invitation, this should be fixed now.
- `invitation_url` when creating an implicit invitation using `/connections/create-invitation` didn't include endpoint, this should be fixed now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-12 15:10:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1969" class=".btn">#1969</a>
            </td>
            <td>
                <b>
                    Changelog and version updates for version 0.7.5-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 19:42:46 +0000 UTC
    </div>
</div>

