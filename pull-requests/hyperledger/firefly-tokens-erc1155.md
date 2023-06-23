---
layout: default
title: firefly-tokens-erc1155
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc1155
---

# firefly-tokens-erc1155 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc1155){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Always pass numbers as base 10 to blockchain connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While evmconnect supports base 10 or base 16 inputs, ethconnect only supports numbers in base 10.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 17:32:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/129" class=".btn">#129</a>
            </td>
            <td>
                <b>
                    Return token pool directly from activation if startId/endId specified
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Returns HTTP 200 instead of HTTP 204.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-22 15:50:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Extract a clearer IERC1155Factory interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Split the concept of a "pool factory" (which encompasses a single method and a single event) away from all of the other opinionated spellings in the IERC1155MixedFungible interface.

The parameters of the TokenPoolCreation event have also been altered, but both the old and new parameters will be parsed by the listener.

This also removes some remaining reliance on "instancePath", which is now deprecated and generally not set ("contractAddress" is favored instead).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 20:15:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Package lock v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `npm install` in the `samples/solidity` directory is taking longer than it should on supported node versions as it is having to convert the package lock from v1 to v2 format. The switch to v2 came with npm 7. npm 6 was supported for as long as node 14 was still supported, but node 14 is now EOL.

I've also removed the truffle dependency as it is a large dependency which looks to be superseded by hardhat now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 10:41:08 +0000 UTC
    </div>
</div>

