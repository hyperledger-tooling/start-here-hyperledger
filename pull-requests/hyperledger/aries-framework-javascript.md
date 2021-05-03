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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    feat: add dependency injection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was considerably easier than I thought it would be.

Just DI for now. No extension API yet.

- Used TSyringe. Very lightweight (1 already used dependency)
- Used symbols for interface based injectables. Maybe we want to use base classes later on to make it easier, but I wanted to keep most of the current working intact. Just replace it with DI
- Use `@scoped(Lifecycle.ContainerScoped)` for injection. This is basically a singleton, however only for the current DI container. This means a child container won't share the same instance. Two reasons:
	- The tests were not happy with a singleton (could have bypassed this however)
	- This allows to run two agents side by side and don't have problems with the singletons
- Instead of using `Repository<RecordClass>` we're now using `RecordRepository`. It was very hard to use this pattern. Maybe we can simplify it later on. For now it was easiest to just create a separate repository per record type.


Let me know what you think. I think this will make extension a lot easier moving forward.

Fixes #211 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 22:44:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    feat: Add support for WebSocket transports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is how it works now:
* A mediator takes endpoint for invitation or DidDoc from `config`.
* An edge agent takes endpoint for invitation or DidDoc from `inboundConnection` if it has any.
* The edge agent gets out of band invitation via http request to mediator (http://mediator1.com/invitation). The invitation contains `ws` endpoint because we want to make a connection via WebSocket.
* The edge agent takes an endpoint for outbound communication from invitation or DidDoc. For a connection with another edge agent, it takes an endpoint from `indbound` connection. Therefore it’s the same `ws` endpoint as it is contained in the mediator invitation.

To integrate ws and http servers together and support multiple transports we would need to enable following:
* A mediator sends a different endpoint for mediation to edge agent.
* The edge agent sets the mediation endpoint somewhere else and do not take it from `inbound` connection invitation or DidDoc.

Other notes:
* I set ws endpoint directly in mediator server by editing `config.endpoint` to value `ws://localhost:${PORT}`
* I skip the ws tests. To run them it's needed to change the mediator server to `mediator-ws.ts` (or integrate ws and HTTP together as I mentioned)

Related to #250 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 10:17:18 +0000 UTC
    </div>
</div>

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

