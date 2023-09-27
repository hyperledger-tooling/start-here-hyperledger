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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2520" class=".btn">#2520</a>
            </td>
            <td>
                <b>
                    Update shared components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates to:
- Indy-VDR 0.4 release (with did:indy support)
- Indy-Credx 1.0.3 minimum version
- Askar 0.3.0-dev.1

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-27 16:50:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2519" class=".btn">#2519</a>
            </td>
            <td>
                <b>
                    Fix: Problem Report Before Exchange Established
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes Credential Exchange Protocol v1 Issue #1730 and similar Issue #2512 for v2.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 23:36:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2517" class=".btn">#2517</a>
            </td>
            <td>
                <b>
                    Change arg_parse to always set --emit-new-didcomm-prefix and --emit-new-didcomm-mime-type to true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

Approach used was to accept the parameters, but whether set or not, set corresponding config value to True.

Left the config settings, but updated the help to say not setting the value is not possible.

Didn't change the tests, but added a comment about why the of the old setting is not particularly useful...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-26 21:55:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2516" class=".btn">#2516</a>
            </td>
            <td>
                <b>
                    fix: mediation routing keys as did key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a minor rethink to #2502; as discussed in my comment on that PR, I think I/we went a bit too far with base58 to did:key normalization. This is the minimum set of changes required to fix the two issues.

Fixes #2492.
Fixes #2357.

These changes also cause did:keys to be sent out in mediation grant messages and, subsequently, connections/did exchange as the `routingKeys` in the DID Document. This has interop implications. A big motivator for these changes however is to enable AFJ/Bifold based agents to connect through a public DID with mediation where AFJ/Bifold is expecting did:keys in the routing keys in the endpoint attrib. So this should help push us towards "good" interop and should only break "bad" interop.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 21:24:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2515" class=".btn">#2515</a>
            </td>
            <td>
                <b>
                    refactor: drop mediator_terms and recipient_terms
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Term negotiation was dropped from the coordinate mediation protocol early in the proposal process. Our implementation helped to determine that it should be dropped but predates the decision. The terms support has hung around unused for years. Time to remove it.

Terms will no longer be stored in mediation records but old mediation records should continue to work (the values will just be ignored).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-25 20:46:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2510" class=".btn">#2510</a>
            </td>
            <td>
                <b>
                    Remove unused dependencies
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
        Created At 2023-09-22 21:15:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2509" class=".btn">#2509</a>
            </td>
            <td>
                <b>
                    0.10.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Verified the latest PR (PyDID update) in AATH -- all tests passed. Looking good!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 19:38:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2500" class=".btn">#2500</a>
            </td>
            <td>
                <b>
                    fix: update pydid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will correct the errror reported in #2497.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 16:37:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2499" class=".btn">#2499</a>
            </td>
            <td>
                <b>
                    Use correct rust log level in dockerfiles 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                From issue https://github.com/hyperledger/aries-cloudagent-python/issues/2498

It looks like `warning` is not a valid Rust log level string https://docs.rs/log/latest/log/enum.Level.html
From what I've seen in traction (which deploys using the dockerfile here), this means logs default to INFO level here even though dockerfile is trying to have it at the warn level. (see details in ticket for what I tried out)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 04:12:06 +0000 UTC
    </div>
</div>

