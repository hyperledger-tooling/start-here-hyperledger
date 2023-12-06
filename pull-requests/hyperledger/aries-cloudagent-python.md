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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2651" class=".btn">#2651</a>
            </td>
            <td>
                <b>
                    Update integration tests for anoncreds-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Final update from the `anoncreds-rs` branch, brings across some integration tests, and also includes a bit of cleanup.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2645" class=".btn">#2645</a>
            </td>
            <td>
                <b>
                    feat: add did:jwk resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements a did:jwk resolver. See https://github.com/hyperledger/aries-acapy-plugins/pull/47 for context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 22:07:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2643" class=".btn">#2643</a>
            </td>
            <td>
                <b>
                    Initial migration of anoncreds revocation code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Adds revocation support from the anoncreds-rs branch.  Still a few TODO's but this PR is ready to go and I'll continue the work in the next PR.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 19:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2642" class=".btn">#2642</a>
            </td>
            <td>
                <b>
                    Feat: DIDX Implicit Request auto-accept and Delete OOB Invitation related records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #2644
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 16:57:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2638" class=".btn">#2638</a>
            </td>
            <td>
                <b>
                    fix: update broken demo dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couldn't proceed with further local testing on my host. Probably due to differences in python versions. 

```
    self.proc = await asyncio.wait_for(future, 20, loop=loop)
                      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
TypeError: wait_for() got an unexpected keyword argument 'loop'
```

But pip install works fine now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 14:22:52 +0000 UTC
    </div>
</div>

