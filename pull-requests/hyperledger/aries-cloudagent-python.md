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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1120" class=".btn">#1120</a>
            </td>
            <td>
                <b>
                    allow for no body
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 13:06:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1118" class=".btn">#1118</a>
            </td>
            <td>
                <b>
                    make long strings look like elsewhere in aca-py; cover new routes code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 11:36:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1116" class=".btn">#1116</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1115" class=".btn">#1115</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1112" class=".btn">#1112</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1111" class=".btn">#1111</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1110" class=".btn">#1110</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1107" class=".btn">#1107</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1105" class=".btn">#1105</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1102" class=".btn">#1102</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1101" class=".btn">#1101</a>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1100" class=".btn">#1100</a>
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

