---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2430" class=".btn">#2430</a>
            </td>
            <td>
                <b>
                    docs(weaver/samples): pin solc to v0.8.8 and turn off IR for Besu asset exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Without having it pinned to v0.8.8, some breaking changes that solc
has snuck in [1] [2] around v0.8.15 (for IR) are breaking the contract
deployment in a way that opcodes end up in the migration contract's
constructor that Besu does not recognize ("opcode INVALID" in the besu
logs if you set the log level to "ALL") in the Besu logs and then sends
back an "internal error" message via the JSON-RPC response, which is a
bug IMO it should state that the user input was invalid (user input
being the contract)
2. Disabled IR in the truffle (solc) config which is a step backwards
because it's a new feature of the solidity compiler that has certain
benefits to it compared to the legacy compilation mode, but enabling it
breaks the build so it just had to be done. In the future if someone
has time to do a deep dive on why exactly it's failing, then it should
be re-enabled because having the legacy compilation mode being our default
is technical debt that should be paid off rather sooner than later because
we never know how it will come back to cause different issues later on.

When IR is enabled, the following error occurs (even on the pinned v0.8.8 solc):
> Compiling ./contracts/transferInterface.sol
> YulException: Variable var_amount_3290 is 9 slot(s) too deep inside the stack.

[1] https://docs.soliditylang.org/en/v0.8.15/ir-breaking-changes.html#semantic-only-changes
[2] https://github.com/ethereum/solidity/issues/13311#issuecomment-1199274310

Fixes #2423

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 01:58:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2429" class=".btn">#2429</a>
            </td>
            <td>
                <b>
                    chore(release): publish v2.0.0-alpha.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Another release to test the deployment workflows.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 06:50:52 +0000 UTC
    </div>
</div>

