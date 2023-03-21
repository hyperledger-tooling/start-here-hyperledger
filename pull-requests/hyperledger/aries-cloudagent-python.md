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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2173" class=".btn">#2173</a>
            </td>
            <td>
                <b>
                    Add support for JsonWebKey2020 for the connection invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added support for the JsonWebKey2020 OKP keys for connection invitations.
To avoid extensive refactoring this is done by converting it to the supported base58 format.

Please, give feedback.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 09:37:20 +0000 UTC
    </div>
</div>

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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2166" class=".btn">#2166</a>
            </td>
            <td>
                <b>
                    fix: run only on main, forks ok
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue #2152 (https://indicio.atlassian.net/browse/ACAP-1004)

I did not include an environment variable, as GitHub seems to throw up its hands when you put it in the workflow file. There seems to be a workaround if you put the variable in .env, but I'm not sure if we want that though...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 17:52:59 +0000 UTC
    </div>
</div>

