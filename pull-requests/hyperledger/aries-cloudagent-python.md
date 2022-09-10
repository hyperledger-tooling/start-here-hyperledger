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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1935" class=".btn">#1935</a>
            </td>
            <td>
                <b>
                    Delete sonarcloud.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Disable automatic sonarcloud

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 15:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1934" class=".btn">#1934</a>
            </td>
            <td>
                <b>
                    Fix/endpoint attrib structure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the solution discussed in #1928 to resolve an issue with the endpoint attrib structure. We have brought the structure into alignment with the did:sov specification by removing the nested endpoint structure and ensuring that service types `profile` and `linked_domains` can be used. This solution is interoperable with AFJ, which also supports endpoint attrib data in the following manner:

```json
{
  "endpoint": "https://example.com",
  "types": ["did-communication", ...],
  "routingKeys": [...],
  "profile": "https://example.com/profile",
  "linked_domains": "https://example.com/linked-domains",
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 23:32:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1933" class=".btn">#1933</a>
            </td>
            <td>
                <b>
                    fix: failed connectionless proof request on some case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In demo menu (2a) connectionless proof request, If a mobile agent (for instance Trinsic) does not include Accept header when calling proof request url, the demo would fail.

Signed-off-by: kukgini <kukgini@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-08 10:34:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1931" class=".btn">#1931</a>
            </td>
            <td>
                <b>
                    Rework on ACA-Py to achieve ledger agnosticism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request contains all the rework that we, as IBM Research, have done on `aries-cloudagent-python` (also known as ACA-Py) with a view to achieve *ledger agnosticism*.
The biggest problem we found out in ACA-Py is that, once the agent is started, the ledger sdk to use is strictly bounded with the `--wallet-type` parameter. More specifically, by choosing a specific wallet (e.g. `--wallet-type indy`) we are bounded to use `IndySdkLedger` as class implementation of the abstract class `BaseLedger`. With this approach we need to create a new wallet whenever we want to support a new ledger:

![ledgerAgnosticBefore](https://user-images.githubusercontent.com/26608445/188931906-ade1950d-c4aa-4d55-b96f-5fb53cdce85e.svg)

We believe that such behaviour goes against the goal of being *ledger agnostic* and here we propose our solution.

In our implementation the user can select what ledger to use by adding a new command-line parameter named `--wallet-ledger`. In this way we can add new ledger implementations without being forced to add a new wallet:

![ledgerAgnosticAfter](https://user-images.githubusercontent.com/26608445/188931931-50f2de5c-21b8-40e6-a106-d6f89d6ee091.svg)

More in details:
- each ledger class implementation (called also as *ledger adapter* class) of the abstract class `BaseLedger` has a `BACKEND_NAME` parameter which is used as the ledger class identifier. Such identifier can be indicated with the `--wallet-ledger` command-line parameter to choose what ledger adapter to use when running the agent;
- we implemented a class named `LedgerProvider` in charge of choosing what ledger class to use to interact with the ledger based on both the parameters `--wallet-type` and `--wallet-ledger`. The choice of the ledger is still bounded to the wallet the user chooses since each wallet can be free to specify what ledgers to interact with. The list of ledgers supported by a specific wallet is defined directly inside the `LedgerProvider` class as `WALLET_SUPPORTED_LEDGERS`;
- we made a rework on the interactions between the agent and the `tails server` to allow revocation in a ledger-agnostic way. Specifically we added the field `ledger_type` into the request payload which goes from the agent to the tails server and which allows the latter to correctly setup his connection with the ledger. To have a ledger-agnostic implementation of the tails-server capable of parsing correctly this new request layout we recommend to use the implementation available [here](https://github.com/pasquale95/indy-tails-server/tree/feature/ledger_agnosticism).

More details can be found at the [LedgerAgnosticism](https://github.com/pasquale95/aries-cloudagent-python/blob/feature/ledger_agnosticism/docs/GettingStartedAriesDev/LedgerAgnosticism.md) document.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-07 16:36:58 +0000 UTC
    </div>
</div>

