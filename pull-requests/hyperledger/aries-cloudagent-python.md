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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2207" class=".btn">#2207</a>
            </td>
            <td>
                <b>
                    0.8.1
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
        Created At 2023-04-05 22:39:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2206" class=".btn">#2206</a>
            </td>
            <td>
                <b>
                    BREAKING: Auto-remove flags for Presentation Exchanges
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The current `--preserve-exchange-records` configuration argument supports credential exchanges only. This PR introduces a new configuration for presentation exchanges and roles within those exchanges. 

We want to preserve existing default behaviour: credential exchanges are removed, and presentation exchanges are stored. The credential exchanges could be saved by setting the'- preserve-exchange-records' configuration. Further override (to the issuer) specifies `auto_remove` in specific API payloads.

The default behaviour remains (credential exchanges removed, presentation exchanges stored) with addition of specifying default removal behaviour for each exchange and role. Since the API payloads use `auto_remove=True/False`, the new configurations are named `--auto-remove-*` and require a "boolean" value: true means remove, and false means store.

Truthy values are: `yes`, `true`, `t`, `y`, and `1`.
Falsey values are: `no`, `false`, `f`, `n`, and `0`.

Values are not case-sensitive.

**Command line Arguments**

```
--auto-remove-cred-exch-records-issuer <boolean value>
--auto-remove-cred-exch-records-holder <boolean value>
--auto-remove-pres-exch-records-verifier <boolean value>
--auto-remove-pres-exch-records-prover <boolean value>
```

**Environment Variables**

```
ACAPY_AUTO_REMOVE_CRED_EXCH_RECORDS_ISSUER=<true/false>
ACAPY_AUTO_REMOVE_CRED_EXCH_RECORDS_HOLDER=<true/false>
ACAPY_AUTO_REMOVE_PRES_EXCH_RECORDS_VERIFIER=<true/false>
ACAPY_AUTO_REMOVE_PRES_EXCH_RECORDS_PROVER=<true/false>
```

The `--preserve-exhange-records` argument is deprecated but still accepted. It is equivalent to:

```
--auto-remove-cred-exch-records-issuer false
--auto-remove-cred-exch-records-holder false
```

If none of the arguments are specified (system default) is equivalent to:

```
--auto-remove-cred-exch-records-issuer true
--auto-remove-cred-exch-records-holder true
--auto-remove-pres-exch-records-verifier false
--auto-remove-pres-exch-records-prover false
```

Once arguments are parsed, the settings are:

```
settings.get("auto_remove_cred_exch_records_issuer")
settings.get("auto_remove_cred_exch_records_holder")
settings.get("auto_remove_pres_exch_records_verifier")
settings.get("auto_remove_pres_exch_records_prover")
```

These settings should **always** be `True` or `False`, not `None`.


**Important**

While testing the previous behaviour, some stray credential exchanges remained when the system was set with `auto_remove = True` and API payload with no field named `auto_remove` to override the default behaviour.  Hopefully, no systems were built to take advantage of this unintended behaviour.


Fixes #2126 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 22:06:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2204" class=".btn">#2204</a>
            </td>
            <td>
                <b>
                    Add Explicit/Offline marking mechanism for Upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2201 
- Pending extensive testing with docker-test scripts

In the config, `explicit_upgrade` is the flag or key and it's value can be `critical` [meaning error and stop] or `warning` [log and proceed]. ~~With `warning`, if there are versions which are not marked as explicit and are in scope for applying the upgrade then upgrade for these versions will proceed [after that it will continue the ACA-Py start up process].~~ With warning, if there are version which are not marked as explicit and are in scope for applying the upgrade then no upgrade will be performed and version in storage not updated.

```
"v0.7.2": {
    ...,
    "explicit_upgrade": "warning",
},
"v0.7.3": {
    ...,
    "explicit_upgrade": "critical",
},
"v0.7.1": {
    ...,
},
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 02:52:03 +0000 UTC
    </div>
</div>

