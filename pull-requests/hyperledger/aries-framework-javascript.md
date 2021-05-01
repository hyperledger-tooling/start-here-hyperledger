---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    feat: add credential info to access attributes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #190
Fixes #187

Example:

```ts
// credentialRecord.getCredentialInfo()
{
  claims: {
    name: 'Timo',
    date_of_birth: '1998-07-29',
    'country-of-residence': 'The Netherlands',
    'street name': 'Test street',
    age: '22',
  },
  metadata: {
    credentialDefinitionId: 'Th7MpTaRZVRYnPiabds81Y:3:CL:17:TAG',
    schemaId: 'TL1EaPFCZ8Si5aUrqScBDt:2:test-schema-1599055118161:1.0',
  },
}
```

```ts
// credentialInfo.getFormattedClaims()
{
  Age: '22',
  'Country Of Residence': 'The Netherlands',
  'Date Of Birth': '1998-07-29',
  'Street Name': 'Test street',
  Name: 'Timo',
}
```


```ts
const credentialInfo = credentialRecord.getCredentialInfo()
const claims = credentialInfo.claims
const formattedClaims = credentialInfo.getFormattedClaims()
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-01 12:31:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    feat: automatic transformation of record classes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transform record classes and its sub objects using class transformer.

Fixes #106


Was sort of a blocker for some of the work I wanted to do for #187, and it was long overdue this was fixed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:13:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    Mediation by Mediator Coordination Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Comes from #249 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 16:31:20 +0000 UTC
    </div>
</div>

