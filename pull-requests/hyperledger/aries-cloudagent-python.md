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
- Does not support encoding of ports in DIDs yet (e.g. `did:web:localhost%3A8443 -> https://localhost:443/.well-known.did.json` yet, because pyDID does not allow '%' char in DID (See: https://github.com/dbluhm/pydid/issues/34)
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1213" class=".btn">#1213</a>
            </td>
            <td>
                <b>
                    Support indy 1.16 predicate restrictions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Still to work out:
* general WQL (+ `"$and"`) for restrictions in proof request requested attributes/predicates
* not necessarily relying on these being a list: they can be a (WQL statement) dict or a list of (WQL statement) dicts, each (WQL statement) dict possibly being its own compound WQL statement; e.g., this is a valid restriction:
```
{
  "$and": [
    {
      "$or": [
        {
          "schema_name": "membership"
        },
        {
          "schema_name": "members"
        }
      ]
    },
    {
      "$neq": {
        "schema_version": "0.1"
      }
    },
    {
      "issuer_did": "abc123"
    },
    {
      "$not": {
        "$in": {
          "attr::name::value": [
            "joe",
            "dolly",
            "bill"
          ]
        }
      }
    }
  ]
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 18:26:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1212" class=".btn">#1212</a>
            </td>
            <td>
                <b>
                    Finish prob rept adoption into issue cred present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 14:43:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1209" class=".btn">#1209</a>
            </td>
            <td>
                <b>
                    Fix exposing wallet storage creds in configuration endpoint.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #1208 

Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 09:19:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1204" class=".btn">#1204</a>
            </td>
            <td>
                <b>
                    Fix: Public Connections Invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1203 
- Went through the following test cases, all invitations should now work as expected.
![image](https://user-images.githubusercontent.com/9292265/119702684-942f2480-be0a-11eb-9527-cbff0e26f885.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 17:11:00 +0000 UTC
    </div>
</div>

