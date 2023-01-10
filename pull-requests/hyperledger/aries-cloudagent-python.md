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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2071" class=".btn">#2071</a>
            </td>
            <td>
                <b>
                    Improved validation of record attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We ran into the issue that our generated client would throw an exception whenever a CredExRecord was deleted. The reason was the record's state parameter being set to "deleted" - a value which is not in the set of allowed values as per the swagger definition.

Changes:
- `STATE_DELETED` attribute added to BaseRecord
- added a function which lists the values of all attributes that start with a common prefix (e.g. `"STATE_"`), optionally including inherited attributes. The resulting list can be used for validation.

I took the occasion to clean up validation a bit (conn-, cred_ex- and pres_ex_records) and add it where it was missing (OobRecord).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 13:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2067" class=".btn">#2067</a>
            </td>
            <td>
                <b>
                    feat: enable creation of DIDs for all registered methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Here're a couple of changes leveraging the recent addition of the `DIDMethods` registry.
The aim is to allow agents using DID methods defined in plugin to create DIDs without implementing method-specific endpoints if not necessary.

Changes:
   * Relax condition on did format for the `POST /wallet/did` endpoint
   * Validate new DIDs parameters using `DIDMethods` in Askar and InMemory profiles
      validate new DIDs parameters
   * Factorize some validation code

Notes:
   * A lot of tests are impacted by the change, if anybody has a suggestion for a quick solution to avoid that...
   * It would be nice to implement the DID derivation in each `DIDMethod` but this would require quite some work to be able to remove the did:sov and did:key initialization hardcoded in `DIDMethods`.

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 07:12:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2066" class=".btn">#2066</a>
            </td>
            <td>
                <b>
                    Update github actions dependencies (for node16 support)
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
        Created At 2023-01-04 20:15:08 +0000 UTC
    </div>
</div>

