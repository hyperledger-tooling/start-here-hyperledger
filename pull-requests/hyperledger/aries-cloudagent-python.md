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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2170" class=".btn">#2170</a>
            </td>
            <td>
                <b>
                    BREAKING: feat: get queued outbound message in transport handle message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will enable queues to annotate outbound messages with relevant context for things like dead letter queues that know which wallet sent the message that failed, what message was being sent, etc.

This is a breaking change for plugins adding queue implementations (cc @shaangill025) but we think this is worthwhile for the ability to improve internal error handling.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 14:52:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2169" class=".btn">#2169</a>
            </td>
            <td>
                <b>
                    0.8.0 release
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
        Created At 2023-03-14 22:27:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2163" class=".btn">#2163</a>
            </td>
            <td>
                <b>
                    Remove CircleCI Status since we aren't using CircleCI anymore
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
        Created At 2023-03-14 02:38:33 +0000 UTC
    </div>
</div>

