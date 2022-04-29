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
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Fix approval event transformation for ERC721
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #55
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 17:08:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Add FFTM_URL config option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support https://github.com/hyperledger/firefly-transaction-manager

Note currently only used for `SendTransaction` API calls when set.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 12:06:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Fix Dockerfile and .dockerignore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 16:17:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Compile contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a compiled TokenFactory contract to the docker image, as well as the source (and dependencies) that were used to compile it. This accomplishes two things:
- Allows the FireFly CLI to deploy the compiled token factory
- Allows the FireFly CLI to point the end user at the source code for the contract that it deployed

This also changes to use a multi-stage Docker build which significantly cuts down on the final image size.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 20:58:38 +0000 UTC
    </div>
</div>

