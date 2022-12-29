---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1123" class=".btn">#1123</a>
            </td>
            <td>
                <b>
                    Add ability to bind a contract interface to a token pool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16).
Depends on https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/104.

_Discussion about the overall architecture/usefulness of this proposed feature should be directed to [FIR-16](https://github.com/hyperledger/firefly-fir/pull/16), while discussion here should focus on specific technical details of the current proposed approach._

This demonstrates a thin thread whereby FireFly can provide ABI details to a token connector, making it easier for the token connector to know the shape of the underlying contract it is dealing with (vs. having to probe/guess at the methods available).

With this change and the corresponding token connector changes, I was able to generate a custom ERC721 with auto-indexing via https://wizard.openzeppelin.com (a variant never previously supported) and successfully mint tokens.

**Outstanding Problems/Questions**
1. ABI format should not be assumed - it should either be configured in the token plugin configuration, or should be queried somehow from the token connector.
2. When creating a token pool, we should probably allow passing the interface by name/version in addition to by ID (similar to the flow when creating contract APIs).
3. We likely want a handshake protocol between FireFly and the token connector in order to prune down the ABI methods it cares about, rather than passing them all on every HTTP request (even a simple contract ABI may be 3KB or more, while a single method definition is around 150 bytes).
4. When ABI format is needed by the token connector, perhaps FireFly should store the converted method definitions rather than converting on demand before every operation.

**Other Misc Notes**
* This feature is only useful to users who have significant knowledge of the underlying token contract that sits on the other side of their token connector.
* It's likely to be most useful when creating a pool against a pre-deployed contract - ie when passing `config.address`. Worth mentioning that FireFly doesn't really "know" you can create pools against pre-deployed contracts (as `config` is opaque), but it's up to the user to understand the combination of features that are useful here.
* Theoretically you could create a factory contract that deploys custom ERC20/ERC721 instances, and then you'd need to pass `interface` on every pool creation even while relying on the factory sitting on the other side of the token connector to do the deploy. Seems like a less useful combo, but calling it out here for completeness.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-28 21:38:00 +0000 UTC
    </div>
</div>

