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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1210" class=".btn">#1210</a>
            </td>
            <td>
                <b>
                    BUG FIX: set connections metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Due https://github.com/hyperledger/aries-cloudagent-python/pull/1186#issuecomment-849452360 

There was a bug that does not save the metadata into the records once they were set.
This PR fixes that bug, updating the connections metadata everywhere.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 11:25:35 +0000 UTC
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1202" class=".btn">#1202</a>
            </td>
            <td>
                <b>
                    Updates to OOB InvitationMessage & Endpoint example - Consistent with RFC0434
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1138 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-24 11:17:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1200" class=".btn">#1200</a>
            </td>
            <td>
                <b>
                    Changes in Endorser Protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request consists of the following changes in endorser protocol : 

1.  The author can give the functionality to the endorser where he/she can auto-write the transaction to the ledger after it gets endorsed.
2. The agent from where the transaction is written to the ledger is separated, it the author writes the transaction, it would go from author's agent and same for endorser.
3. Always, the record would be stored in author's wallet, irrespective of who (Author/Endorser) actually writes the transaction to the ledger.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-22 19:12:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1199" class=".btn">#1199</a>
            </td>
            <td>
                <b>
                    fix cascading problem report, error state failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sorry about that
Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-21 21:44:10 +0000 UTC
    </div>
</div>

