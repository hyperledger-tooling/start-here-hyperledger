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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1224" class=".btn">#1224</a>
            </td>
            <td>
                <b>
                    Integration test for endorsement with credential issue and revocation…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … w.i.p.

Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-05 15:55:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1223" class=".btn">#1223</a>
            </td>
            <td>
                <b>
                    run_demo fails if ../logs folder doesn't exist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Steps to reproduce:
1. Clone repo
2. `cd demo`
3. `run_demo faber`

Expected:
- to start the demo connection flow

Actual:
- fails with:

```
./run_demo faber                                             
Preparing agent image...
sha256:5c8d0c8453ec05bcd7ff2e234267e09e113ac041707cb4f21a22f613f832727c
Trying to detect ngrok service endpoint
jq not found
192.168.65.3
docker: Error response from daemon: Mounts denied: 
The path ..../aries-cloudagent-python/demo/../logs
is not shared from OS X and is not known to Docker.
You can configure shared paths from Docker -> Preferences... -> File Sharing.
See https://docs.docker.com/docker-for-mac/osxfs/#namespaces for more info.
.
ERRO[0000] error waiting for container: context canceled 
```

The proposed fix assumes that `logs` are only required when `--timing` in enabled.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-05 13:05:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1220" class=".btn">#1220</a>
            </td>
            <td>
                <b>
                    Feature/didx request with public did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces an optional flag `use_public_did` in `/didexchange/create-request`

Enabling the flag will create a DIDX request with the public DID of the requester.
The approach is not ideal since the did doc will still be attached to the request instead of just setting the `did` property as suggested in the [RFC](https://github.com/hyperledger/aries-rfcs/blob/master/features/0023-did-exchange/README.md#request-message-attributes) (but not required :) ).

Setting only the `did` property leads to issues because of inconsistencies in ACA-Py's DID Doc class and the DID Doc class returned by the resolver. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 13:28:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1218" class=".btn">#1218</a>
            </td>
            <td>
                <b>
                    Feature/native did web resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add native [did:web](https://w3c-ccg.github.io/did-method-web/) resolver. Carved out and touched up from #1143 

- Uses DID and DID Doc validation from pyDID
- ~Does not support encoding of ports in DIDs yet (e.g. `did:web:localhost%3A8443 -> https://localhost:443/.well-known/did.json` yet, because pyDID does not allow '%' char in DID (See: https://github.com/dbluhm/pydid/issues/34)~
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 09:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1216" class=".btn">#1216</a>
            </td>
            <td>
                <b>
                    Add outofband credential-offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The out of band protocol doesn't support the attachment type credential-offer yet. I added my code in outofband receive_invitation to receive a credential offer and send a credential request. 

The receive_offer and create_request functions worked perfectly , But I am facing a `connection_record not found error` while the issuer agent executes credential_request_handler script. I am including the logs below. 

`  

> File "/home/indy/aries_cloudagent/core/dispatcher.py", line 198, in handle_message
>     await handler(context, responder)
>   File "/home/indy/aries_cloudagent/protocols/issue_credential/v1_0/handlers/credential_request_handler.py", line 39, in handle
>     context.message, context.connection_record.connection_id
>   File "/home/indy/aries_cloudagent/protocols/issue_credential/v1_0/manager.py", line 470, in receive_request
>     session, connection_id, message._thread_id
>   File "/home/indy/aries_cloudagent/protocols/issue_credential/v1_0/models/credential_exchange.py", line 206, in retrieve_by_connection_and_thread
>     {"connection_id": connection_id} if connection_id else None,
>   File "/home/indy/aries_cloudagent/messaging/models/base_record.py", line 250, in retrieve_by_tag_filter
>     cls.__name__, tag_filter, f", {post_filter}" if post_filter else ""
> aries_cloudagent.storage.error.StorageNotFoundError: V10CredentialExchange record not found for {'thread_id': '56ccbd83-3800-41a8-907c-fcbedeebb706'}, {'connection_id': '737ca643-7f05-470a-8b47-89fafb11a83d'}

`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 12:30:09 +0000 UTC
    </div>
</div>

