---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3429" class=".btn">#3429</a>
            </td>
            <td>
                <b>
                    feat: add did core support in resolving service endpoints function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mykhailo Sizov <mykhailo.sizov@securekey.com>

**Title:**
Add did core support in resolving service endpoints function

**Description:**
Solves: https://github.com/hyperledger/aries-framework-go/issues/3428

**Summary:**
Added support of the next structure of service in DID:
```
"service": [
    {
      "id": "#linkeddomains",
      "type": "LinkedDomains",
      "serviceEndpoint": {
        "origins": [
          "https://did.rohitgulati.com/"
        ]
      }
    },
    {
      "id": "#hub",
      "type": "IdentityHub",
      "serviceEndpoint": {
        "instances": [
          "https://hub.did.msidentity.com/v1.0/a492cff2-d733-4057-95a5-a71fc3695bc8"
        ],
        "origins": []
      }
    }
  ]
```

Covered in unit test here: https://github.com/hyperledger/aries-framework-go/blob/main/pkg/doc/didconfig/interop_test.go#L37


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-08 17:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3427" class=".btn">#3427</a>
            </td>
            <td>
                <b>
                    chore: Service priority should be an interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Service.Priority should be an interface so it can be omitted if not set.

Closes #3426

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 23:35:09 +0000 UTC
    </div>
</div>

