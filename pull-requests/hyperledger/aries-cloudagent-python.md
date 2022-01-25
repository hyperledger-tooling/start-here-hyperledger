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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1610" class=".btn">#1610</a>
            </td>
            <td>
                <b>
                    Fixes for v7.3.0 - Issue#1597
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
- resolve #1597 
- Fixes (1)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 17:00:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1607" class=".btn">#1607</a>
            </td>
            <td>
                <b>
                    Auto-promote author did to public after endorsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a couple of options:

Author can specify to auto-promote DID to their public DID when they receive the endorsed transaction (and it is saved)

Endorser can use a different DID for endorsing than they use for their public DID (for connections) (can be specified globally by parameter, or can be specified when they call the endorse endpoint).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 17:47:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1606" class=".btn">#1606</a>
            </td>
            <td>
                <b>
                    Update aiohttp dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## What is this PR for?

- Update aiohttp and async-timeout dependency
- aiohttp 3.7 has https://github.com/aio-libs/aiohttp/issues/4818 exploit
- Changes were tested with all jsonld based flows
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 08:55:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1605" class=".btn">#1605</a>
            </td>
            <td>
                <b>
                    Replace blank credential/presentation exchange states with abandoned state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to #1588 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 19:33:56 +0000 UTC
    </div>
</div>

