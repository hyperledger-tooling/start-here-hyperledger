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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1926" class=".btn">#1926</a>
            </td>
            <td>
                <b>
                    Endorser doc updates and some bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Fixes a couple of issues with DID ATTRIB transactions, and adds some technical docs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 19:22:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1925" class=".btn">#1925</a>
            </td>
            <td>
                <b>
                    Fix: the type of tails file path to string.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi.

This PR corrects the type of tails file path.

`self.tails_local_path` must be a string. However, it was assigned a PosixPath value.

So I got the below error.
`TypeError: bytes or integer address expected instead of PosixPath instance`

At here.
https://github.com/hyperledger/indy-shared-rs/blob/main/wrappers/python/indy_credx/bindings.py#L797

Thanks!

Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 05:05:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1924" class=".btn">#1924</a>
            </td>
            <td>
                <b>
                    Pre-populate revoc_reg_id on IssuerRevRegRecord
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This avoids having a confusingly blank `revoc_reg_id` on the record in the `init` state.

Registries in the `init` state are also filtered from the `/revocation/registries/created` endpoint.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 18:15:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1922" class=".btn">#1922</a>
            </td>
            <td>
                <b>
                    fix: propagate endpoint from mediation record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves a bug in #1899 in which the public DID endpoint of an agent behind a mediator was the agent's own endpoint. These changes ensure that a mediated agent's public DID endpoint is the mediator's endpoint.

Signed-off-by: Char Howland <char@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 18:20:09 +0000 UTC
    </div>
</div>

