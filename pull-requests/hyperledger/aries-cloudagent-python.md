---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python

You can clone this repo on <span class="fs-3">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1116](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1116)
            </td>
            <td>
                <b>
                    Changes in Endorser Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a PR that contains changes in endorser protocol.

The changes are defined in the issue
#1040 
#1028 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-24 11:13:48 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1115](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1115)
            </td>
            <td>
                <b>
                    Add generic JWE envelope handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This decouples the in-memory pack/unpack from the envelope handling code, to allow other encryption methods in future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 23:02:21 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1112](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1112)
            </td>
            <td>
                <b>
                    Feature/secure comparison
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>

compare_digest only supports ascii strings or bytes like objects. I added .encode() method to the compare_digest to allow utf string to be compared.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 21:01:56 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1111](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1111)
            </td>
            <td>
                <b>
                    secured api_key against timing attacks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wadeking98 <wkingnumber2@gmail.com>
@andrewwhitehead 
comparing user input to secrets and then responding makes this application vulnerable to timing attacks. See resource here: https://blog.sqreen.com/developer-security-best-practices-protecting-against-timing-attacks/  
  
While an attacker isn’t likely to be able to exploit this from somewhere over the internet due to network jitter, they might be able to pull it off if the agent ever supports TOR, HTTP/2 (timeless timing attack), or if they get access to a pod inside the same openshift cluster that can send requests to the agent (ie: the api pod)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 19:00:50 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1110](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1110)
            </td>
            <td>
                <b>
                    Issue cred bound counter offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/aries-cloudagent-python/issues/1103
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 14:18:40 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1107](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1107)
            </td>
            <td>
                <b>
                    Fixes for JSON-LD routes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Had a few bugs slip past; discovered these after more manual testing. This PR activates the json-ld routes, makes the DID resolver DID Document validation less picky, and corrects a schema validation issue in `verify`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 04:27:48 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1105](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1105)
            </td>
            <td>
                <b>
                    Update package dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 03:22:59 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1102](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1102)
            </td>
            <td>
                <b>
                    make clear that presentation violates restrictions either proposed or…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … requested

Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 14:29:41 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1101](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1101)
            </td>
            <td>
                <b>
                    Fix introductions protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix introductions protocol. Integrate did-exchange problem reports with problem-report protocol (leave connections as per its RFC 160, predating problem-report protocol).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 14:01:59 +0000 UTC
    </div>
</div>

<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1100](https://api.github.com/repos/hyperledger/aries-cloudagent-python/pulls/1100)
            </td>
            <td>
                <b>
                    Replace ledger with resolver in OOB manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 02:40:51 +0000 UTC
    </div>
</div>

