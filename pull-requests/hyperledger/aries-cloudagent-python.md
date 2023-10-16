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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2548" class=".btn">#2548</a>
            </td>
            <td>
                <b>
                    Update .readthedocs.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Another fix to this YAML file. Unfortunately, I can't test it without getting it into main (AFAIK...).  Frustrating...

Errors were dumb in the last try...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-15 20:16:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2547" class=".btn">#2547</a>
            </td>
            <td>
                <b>
                    Update .readthedocs.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RTD is broken because (I think) missing section of RTD.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-14 22:56:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2546" class=".btn">#2546</a>
            </td>
            <td>
                <b>
                    DRAFT: please_ack support PoC for the 0453-issue-credential-v2 protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is PoC code for the PR#2540 (https://github.com/hyperledger/aries-cloudagent-python/pull/2540). It shows possible implementation of the `please_ack` decorator support ('option 2' in the document in the PR#2540)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 11:23:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2545" class=".btn">#2545</a>
            </td>
            <td>
                <b>
                    :art: clarify LedgerError message when TAA is required and not accepted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously:
```py
            if await self.is_ledger_read_only():
                raise LedgerError(
                    "Error cannot write cred def when ledger is in read only mode"
                )
```

`is_ledger_read_only` also checks to see if TAA is required, and if not accepted it will also report the ledger is read-only:
```py
    async def is_ledger_read_only(self) -> bool:
        """Check if ledger is read-only including TAA."""
        if self.read_only:
            return self.read_only
        # if TAA is required and not accepted we should be in read-only mode
        taa = await self.get_txn_author_agreement()
        if taa["taa_required"]:
            taa_acceptance = await self.get_latest_txn_author_acceptance()
            if "mechanism" not in taa_acceptance:
                return True
        return self.read_only
```

To make this clearer to the user, I updated the relevant error messages to say TAA  may also be the cause of the LedgerError.

e.g.:
```py
                raise LedgerError(
                    "Error cannot write cred def when ledger is in read only mode, "
                    "or TAA is required and not accepted"
                )
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 09:34:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2544" class=".btn">#2544</a>
            </td>
            <td>
                <b>
                    fix: correct minor typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes some minor spelling typos:

   Congradulations -> Congratulations
   explicitely -> explicitly
   supprting -> supporting

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 13:33:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2541" class=".btn">#2541</a>
            </td>
            <td>
                <b>
                    Anoncreds-rs pytest update (Credential Definitions)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                This is the first set of updates for credential definitions API only.

Since we have not updated/implemented endorser in the anoncreds-rs branch, I have left endorser related tests as skipped.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 18:30:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2540" class=".btn">#2540</a>
            </td>
            <td>
                <b>
                    DRAFT: PleaseAck.md document
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is an attempt to make a start point of discussion how to implement the `please_ack` decorator support in ACA-Py. The PR contains initial version of the document that aims to find the final solution. It contains some thoughts/ideas about possible implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 18:19:17 +0000 UTC
    </div>
</div>

