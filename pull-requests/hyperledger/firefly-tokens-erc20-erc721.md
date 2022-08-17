---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Patched Command Injection in lodash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `lodash` versions prior to 4.17.21 are vulnerable to Command Injection via the template function.

**CVE-2021-23337**
`7.2/ 10`
CVSS:3.1/AV:N/AC:L/PR:H/UI:N/S:U/C:H/I:H/A:H

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 02:23:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Patch ProxyAgent vulnerable to MITM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
`Undici.ProxyAgent` never verifies the remote server's certificate, and always exposes all request & response data to the proxy. This unexpectedly means that proxies can MitM all HTTPS traffic, and if the proxy's URL is HTTP then it also means that nominally HTTPS requests are actually sent via plain-text HTTP between Undici and the proxy server.

## Impact
This affects all use of HTTPS via HTTP proxy using `Undici.ProxyAgent` with Undici or Node's global `fetch`. In this case, it removes all HTTPS security from all requests sent using Undici's `ProxyAgent`, allowing trivial MitM attacks by anybody on the network path between the client and the target server (local network users, your ISP, the proxy, the target server's ISP, etc).
This less seriously affects HTTPS via HTTPS proxies. When you send HTTPS via a proxy to a remote server, the proxy can freely view or modify all HTTPS traffic unexpectedly (but only the proxy).

**CVE-2022-32210**
`7.7/ 10`
CVSS:3.1/AV:N/AC:H/PR:H/UI:N/S:C/C:H/I:H/A:N

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 02:13:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    🐛 BUG: Patched CVE-2022-24434 Crash in HeaderParser in dicer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This affects all versions of package dicer. A malicious attacker can send a modified form to server, and crash the nodejs service. A complete denial of service can be achived by sending the malicious form in a loop.

**CVE-2022-24434**
`7.5/ 10`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 02:10:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    fixing url manipulation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Equivalent of https://github.com/hyperledger/firefly-tokens-erc1155/pull/90

Fixing errors caused by URL manipulation logic described in https://github.com/hyperledger/firefly-tokens-erc1155/issues/53

Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 12:40:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    Pass through EthConnect/EVMConnect receipts unchanged
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Per https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/72#issuecomment-1210782114
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 19:47:01 +0000 UTC
    </div>
</div>

