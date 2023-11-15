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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2605" class=".btn">#2605</a>
            </td>
            <td>
                <b>
                    Default connection_id to None to account for Connectionless Proofs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a small change in response to [this issue and conversation](https://github.com/hyperledger/aries-cloudagent-python/issues/2597).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 21:50:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2604" class=".btn">#2604</a>
            </td>
            <td>
                <b>
                    chore: correct type hints on base record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a small tweak to correct the type hints on base record and related base classes. These are base classes used widely both within ACA-Py and in plugins. Having these types corrected will solve a cascade of static type checking errors.

These aren't strictly necessary errors to fix but they sure make my life as a developer easier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 20:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2603" class=".btn">#2603</a>
            </td>
            <td>
                <b>
                    black formatter extension configuration update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See PR #2602

The black formatter extension was updated last night and the current configuration doesn't work. This simple change corrects the loading error.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 20:04:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2602" class=".btn">#2602</a>
            </td>
            <td>
                <b>
                    Update Devcontainer pytest ruff black
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bring in changes from commit 48e24043f0a5ad89b5e6e808c26b9552a8856abd.

Updates devcontainer to run pytests in Testing view and integrate `ruff` and `black` into the IDE better.

One change is in devcontainer.json, setting the black formatter to "useBundled"...  They updated their extension last night. The change is also needed in the main branch.

```
Published 2022-04-14, 14:24:13
Last released 2023-11-08, 02:11:58
Last updated 2023-11-08, 10:56:39
Identifier ms-python.black-formatter
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 19:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2600" class=".btn">#2600</a>
            </td>
            <td>
                <b>
                    Add ConnectionProblemReport handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Leaving this here as a starting point or example.

See issues #2530 and #2599.

I think we would want to address #2599 first (or include in here) and get the error classes fixed up, then the handler will actually be effective.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-08 16:36:13 +0000 UTC
    </div>
</div>

