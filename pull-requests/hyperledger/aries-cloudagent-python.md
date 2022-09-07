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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1926" class=".btn">#1926</a>
            </td>
            <td>
                <b>
                    Endorser doc updates and some bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Fixes a couple of issues with DID ATTRIB transactions, and adds some technical docs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 19:22:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1925" class=".btn">#1925</a>
            </td>
            <td>
                <b>
                    Fix: the type of tails file path to string.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi.

This PR corrects the type of tails file path.

`self.tails_local_path` must be a string. However, it was assigned a PosixPath value.

So I got the below error.
`TypeError: bytes or integer address expected instead of PosixPath instance`

At here.
https://github.com/hyperledger/indy-shared-rs/blob/main/wrappers/python/indy_credx/bindings.py#L797

Thanks!

Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-02 05:05:09 +0000 UTC
    </div>
</div>

