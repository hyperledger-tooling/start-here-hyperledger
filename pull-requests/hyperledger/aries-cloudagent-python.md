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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1379" class=".btn">#1379</a>
            </td>
            <td>
                <b>
                    Write schema cred def non secrets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In progress - so far it has only been test manually.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 20:04:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1378" class=".btn">#1378</a>
            </td>
            <td>
                <b>
                    Allow underscore in endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR solves issue #1362.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 13:45:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1377" class=".btn">#1377</a>
            </td>
            <td>
                <b>
                    fix: send proposal schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                send-proposal doesn't have `connection_id` in the schema, which is inconvenient for generated clients
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 11:27:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1376" class=".btn">#1376</a>
            </td>
            <td>
                <b>
                    feat: add inject_or
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the `required` parameter from `Injector.inject` and introduces `inject_or` that mimics the behavior of `inject(..., required=False)`. The reasoning for this change is that type checkers take issue with using the result of `inject(..., required=True)` when the signature says that it could still be `None`. For example:

```python
storage = context.inject(BaseStorage)
records = await storage.find_all_records(...)
```
Yields the error `"find_all_records" is not a known member of "None"` when using pyright, even though we know that the call will have resulted in an error if it was actually `None`.

This PR is mostly a proposal and does not yet fix the 109 or so instances of `inject(..., required=False)` that should be switched to `inject_or`. Open to suggestions or alternatives.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 21:16:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1375" class=".btn">#1375</a>
            </td>
            <td>
                <b>
                    fix: refine typing on base record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows type checkers such as pyright to detect that `ConnRecord.retrieve_by_id` returns a `ConnRecord` rather than a `BaseRecord`

These changes are purely cosmetic/developer quality of life improvements.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 20:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1374" class=".btn">#1374</a>
            </td>
            <td>
                <b>
                    Change log for 0.7.1 and update version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 20:29:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1373" class=".btn">#1373</a>
            </td>
            <td>
                <b>
                    Timezone inclusion [ISO 8601] for W3C VC and Proofs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1370
- default timezone: UTC
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 15:47:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1371" class=".btn">#1371</a>
            </td>
            <td>
                <b>
                    Updates to eliminate warnings on RTD doc generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

I added a mock for `aries_cloudagent.vc`, which eliminated all of the errors. Of course I suspect that it also removes the doc generation for that module, but am not certain.  But I feel better that all the warnings are gone...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 16:59:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1368" class=".btn">#1368</a>
            </td>
            <td>
                <b>
                    #1349 Added option to multitenant mode to handle multiple wallets inside the same subwallet with many Askar profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This mode can be run by specifying askar-profile as the wallet_type in the CLI argument --multitenancy-config
Added AskarProfileMultitenantManager class which handles the new logic to get the wallet profile. The old logic was moved to MultitenantManager. The both extend BaseMultitenantManager where most of the previous code remained
The MultitenantManagerProvider chooses the right manager to use depending on the CLI argument
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 08:56:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1366" class=".btn">#1366</a>
            </td>
            <td>
                <b>
                    Documentation and unit test cleanups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-22 22:53:17 +0000 UTC
    </div>
</div>

