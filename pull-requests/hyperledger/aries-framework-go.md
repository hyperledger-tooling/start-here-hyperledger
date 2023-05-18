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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3587" class=".btn">#3587</a>
            </td>
            <td>
                <b>
                    chore: update spi, kmscrypto module dependencies
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
        Created At 2023-05-16 14:59:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3586" class=".btn">#3586</a>
            </td>
            <td>
                <b>
                    perf: reuse same gjson parser
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
        Created At 2023-05-15 11:07:12 +0000 UTC
    </div>
</div>

