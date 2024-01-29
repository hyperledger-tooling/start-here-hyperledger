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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2739" class=".btn">#2739</a>
            </td>
            <td>
                <b>
                    Update BBS+ context to bypass redirections
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
        Created At 2024-01-29 17:30:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2737" class=".btn">#2737</a>
            </td>
            <td>
                <b>
                    bump pydid to v 0.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses #2677

@dbluhm I ran a `poetry update pydid` after changing the version in the `pyproject.toml` file. Seems like it did the trick.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 21:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2734" class=".btn">#2734</a>
            </td>
            <td>
                <b>
                    Upgrade anoncred-rs to version 0.2.0-dev8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still waiting for integration tests locally.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 16:37:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2732" class=".btn">#2732</a>
            </td>
            <td>
                <b>
                    0.12.0rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @dbluhm -- note the update in the documentation for the DID Resolver documentation. I assume that is OK, but didn't actually try it.  I'll try to get to that. I wanted to keep the version updated so that it will be found in a repo search as we publish new releases.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 21:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2731" class=".btn">#2731</a>
            </td>
            <td>
                <b>
                    Relax validation of holder DID when submitting a credential request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See issue https://github.com/hyperledger/aries-cloudagent-python/issues/2714

Relax validation to allow did:peer (or any value) for the holder/prover did on a credential request.

This works with an askar wallet, but anoncreds-askar will fail due to its own did validation (see issue https://github.com/hyperledger/anoncreds-rs/issues/307)

This PR will work once the anoncreds-rs issue is also fixed.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 19:41:06 +0000 UTC
    </div>
</div>

