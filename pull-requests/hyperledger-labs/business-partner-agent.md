---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    w3c interoperability fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing connection and credential protocols against aries-framework-go.

**Fixes:**

- added option to create oob invitations with did:key
- prefixing peer did's with did:peer
- added aca-py's config flags that switch the didcomm mime-type as the wire format is not supported by the go-agent

**Tested:**
- [x] Receive/create oob invitations with did:key works both ways bpa <-> framework-go
- [ ] Receive/create did-exchange invitation - is not working with aca-py as only did:indy is supported
- [ ] Issue/receive w3c credentials

**Go Agent Config in IDE**

Start flags:

```
start --api-host localhost:8081 \
     --database-type mem \
     --inbound-host http@<host-ip>:8082 \
     --inbound-host-external http@http://<host-ip>:8082
     --webhook-url http://<host-ip>:8080/log
     --log-level DEBUG 
     --agent-default-label MyGoAgent
```
Compiler flags:

```
-tags ACAPyInterop
```
Environment:
```
ARIESD_AUTO_ACCEPT=true
```

**Curl against go-agent**

Create did-exchange invitation
```
 curl  -X 'POST' \
  'http://localhost:8081/connections/create-invitation' \
  -H 'accept: application/json' \
  -d ''
```

Create oob invitation:
```
curl -X 'POST' \
  'http://localhost:8081/outofband/create-invitation' \
  -H 'accept: application/json' \
  -H 'Content-Type: application/json' \
  -d '{"label": "Go Agent"}'
```

Receive oob invitation:
```
curl -X POST "http://localhost:8081/outofband/accept-invitation" -H  "content-type: application/json" -d "{\"invitation\":{\"@id\":\"5fa6dc8e-63ed-4af8-ae32-2533c109ea47\",\"@type\":\"https://didcomm.org/out-of-band/1.0/invitation\",\"services\":[{\"id\":\"#inline\",\"type\":\"did-communication\",\"recipientKeys\":[\"did:key:z6MkjHKsXMwNbn1xjG3ge2WWT1Gq7FLeCo2sgRqW5pVgjqdn\"],\"serviceEndpoint\":\"http://<host-ip>:8888\"}],\"handshake_protocols\":[\"https://didcomm.org/didexchange/1.0\"]},\"my_label\": \"aca-py\"}"
```

Get connections
```
curl -X GET "http://localhost:8081/connections" -H  "accept: application/json"
```

Test if connecting to the transport works
```
curl -v -X 'POST' -H 'Content-Type: application/didcomm-envelope-enc'  http://:<host-ip>:8082
```

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/718"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 11:41:21 +0000 UTC
    </div>
</div>

