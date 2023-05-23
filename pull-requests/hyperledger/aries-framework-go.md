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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3592" class=".btn">#3592</a>
            </td>
            <td>
                <b>
                    chore: update component/models version in afgo
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
        Created At 2023-05-23 15:41:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3591" class=".btn">#3591</a>
            </td>
            <td>
                <b>
                    chore: update component dependencies
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
        Created At 2023-05-23 14:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3590" class=".btn">#3590</a>
            </td>
            <td>
                <b>
                    refactor: move presexch to component/models, VDR to component/vdr.
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
        Created At 2023-05-18 22:38:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3588" class=".btn">#3588</a>
            </td>
            <td>
                <b>
                    feat: added JWT handling for limit disclosure Presentation Definition query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Added JWT handling for limit disclosure Presentation Definition query.

**Summary:**
After new credential is created based on limit disclosure constraints:
```
credential, err = createNewCredential(constraints, credentialSrc, template, credential, opts...)
if err != nil {
     return nil, fmt.Errorf("create new credential: %w", err)
}
```
it always returned in JSON-LD format.

Then, down the code, we check is it JWT in `merge` func
```
vcFormat := FormatLDPVC
if credential.JWT != "" {
     vcFormat = FormatJWTVC
}
.....
  desc := &InputDescriptorMapping{
	PathNested: &InputDescriptorMapping{
		Format: vcFormat,
	},
}
```

I added a code that calculates JWT field in limited disclosure VC based on existing claims. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 09:14:32 +0000 UTC
    </div>
</div>

