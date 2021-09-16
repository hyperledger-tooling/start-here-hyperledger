---
layout: default
title: aries-mobile-agent-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-react-native
---

# aries-mobile-agent-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    Fix/aries hooks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

* Fixed a bug throwing `Invalid hook call` related to two copies of `React` running in the app
* Fixed default mediator config to work as previous version
* Fixed state usage in `aries-hooks` to properly update on events
* Brought back `PollingInboundTransporter` to receive messages
* Fixed `Intl` error on Contacts screen
* Other minor fixes

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

Tested with .env file containing
```
MEDIATOR_URL=https://mediator.animo.id
GENESIS_URL=http://dev.greenlight.bcovrin.vonx.io/genesis
```

and using Faber demo Agent from the `https://github.com/hyperledger/aries-cloudagent-python` repository ran on `https://labs.play-with-docker.com` with
```
LEDGER_URL=http://dev.greenlight.bcovrin.vonx.io ./run_demo faber
```

I was able to receive protected text message:
```
 DEBUG  DEBUG: Agent Aries Bifold received message
 INFO  INFO: Received message with type 'https://didcomm.org/messagepickup/1.0/batch' from connection 82a71d4a-f236-4672-80cf-2bbe4e811554 (Animo Mediator) {
  "@type": "https://didcomm.org/messagepickup/1.0/batch",
  "@id": "dad39efc-3f06-4904-939a-a144339ab009",
  "messages~attach": [
    {
      "id": "a36429da-a701-4843-9370-e2a5b4edead4",
      "message": {
        "protected": "eyJlbmMiOiJ4Y2hhY2hhMjBwb2x5MTMwNV9pZXRmIiwidHlwIjoiSldNLzEuMCIsImFsZyI6IkF1dGhjcnlwdCIsInJlY2lwaWVudHMiOlt7ImVuY3J5cHRlZF9rZXkiOiJtaTJqOExKbC1sdXlRM1V2TWlJbFl1amgzS3lXRExITVpHQjBwbDZCQ3FNYjhobnZMcGJIaXFhTFR5cDV4MGgxIiwiaGVhZGVyIjp7ImtpZCI6Ijd3ZjI5OXVmc3c0QUF4d0hmSnYyaU51TDNndXA5cVF2VGlINVFNc1R4QVBIIiwiaXYiOiI5VDFaRnpnZUtIeUNxYzZQM05fMTY1dHZNYThVdFJqUyIsInNlbmRlciI6IjV0ZlhtWFpOZmlpYUpYelNBUWpOV1g1ZGhpMklQZGNlTndHQXZRYzJ2RFBEYlI5Ung4eHM0U2lSbWIyUlVWaXJNN0wwTU9CNlEzOVYyemkwTXBXam9kSm5KTllyalpJT3FhMFpHVTIxbTBlZWRueUF2SURnV3lsRHhnPT0ifX1dfQ==",
        "iv": "JoRQTP8UH7r5n9Ze",
        "ciphertext": "FzQZYetyXrmxKoc05wtlbenZahB5lNq_txjmt7Gldqcf0FR86v8mmLk1s5XdhTCEnz9ZXeFyA1QxhcZ10CrSG18949DcloUvFGNipt9eVFkdC00doqgrBLjmrpffPLGtnyQ1AKmXsQbU5tZrzsQN1Vt0JLdwLtfMgA12mU--9HR6iCT-A-Chhno2UkTRBiCqRkRdebD6jh5w0VsSUC5cGoKkwxtLJxOzW4Xo6xKo6yJo2TJCiPcffcI=",
        "tag": "V5IkDz6MUgrSWttXDu_LMA=="
      }
    }
  ]
}
```
and credentials offer, although this message type is not yet supported:
```
ERROR  AriesFrameworkError: No handler for message type "https://didcomm.org/issue-credential/2.0/offer-credential" found, js engine: hermes
```
Anyway, the connection is working properly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 15:34:58 +0000 UTC
    </div>
</div>

