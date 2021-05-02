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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    feat: add internal http outbound transporter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a first attempt at internalizing the http transport. Only the outbound for now, as it was the easiest. Made two http post implementation so it will work in both RN and Node.JS without having to add another dependency.

You can import it and works out of the box:

```ts
import { Agent, HttpOutboundTransporter } from 'aries-framework'

const agent = new Agent(config)
const httpOutboundTransport = new HttpOutboundTransporter(agent)
agent.setOutboundTransporter(httpOutboundTransport)
```

I made a start at `supportedSchemes`. It is not checked yet, but this allows us to determine the transport to use for a specific message when we add support for multiple transport. That should be a fairly small addition once this is merged. 

Also added an option to specify the didcomm mime type to use. This differs for AIP1.0/AIP2.0.

What do you think?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-01 21:31:39 +0000 UTC
    </div>
</div>

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

