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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2511" class=".btn">#2511</a>
            </td>
            <td>
                <b>
                    Restore aca-py script for when poetry's script support is not suitable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should resolve some edge cases where the poetry script `aca-py` did not fully replace the need for the dedicated script file in `bin/aca-py` mentioned in #2436. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 22:35:29 +0000 UTC
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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2502" class=".btn">#2502</a>
            </td>
            <td>
                <b>
                    fix: mediation webhook routing keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Re: #[2357](https://github.com/hyperledger/aries-cloudagent-python/issues/2357) and #[2492](https://github.com/hyperledger/aries-cloudagent-python/issues/2492)

Indicio PR: https://github.com/Indicio-tech/aries-cloudagent-python/pull/153

Tagging and credit due to @dbluhm 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 19:00:47 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2496" class=".btn">#2496</a>
            </td>
            <td>
                <b>
                    Fix: Ledger error when registering nym after multi-ledger switch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2473 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 16:14:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2495" class=".btn">#2495</a>
            </td>
            <td>
                <b>
                    fix: run tests script copying local env
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the scripts/run_tests script and its dockerfiles to make sure it doesn't copy local .venv directories into the container image. This was causing the script to fail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 18:53:16 +0000 UTC
    </div>
</div>

