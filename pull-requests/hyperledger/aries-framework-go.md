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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3630" class=".btn">#3630</a>
            </td>
            <td>
                <b>
                    feat: change DI VM purpose resolution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using [ResolveSigningVMWithRelationship](https://github.com/hyperledger/aries-framework-go/blob/50313f0971cff8b74e4ad0cb1ce45910f6653352/component/models/jwt/didsignjwt/signjwt.go#L189) function causes a bug in VM relationship verification for Data integrity.

1. For instance, let's take issuer's DID, that after resolving has the following structure:
```
{
  "verificationMethod": [
   ID: "abc",
   .....
  ],
  "authentication": [
   ID: "abc",
   .....
  ]
}
```
3. Function [docRes.DIDDocument.VerificationMethods()](https://github.com/hyperledger/aries-framework-go/blob/50313f0971cff8b74e4ad0cb1ce45910f6653352/component/models/jwt/didsignjwt/signjwt.go#L221) with empty arguments returns a map with 2 elements: key `VerificationRelationshipGeneral` and `Authentication`. 
Values for those keys are verification methods with the same `ID` field.
4. Because func [docRes.DIDDocument.VerificationMethods()](https://github.com/hyperledger/aries-framework-go/blob/50313f0971cff8b74e4ad0cb1ce45910f6653352/component/models/jwt/didsignjwt/signjwt.go#L221) returns a map, the order of elements in `for ... range` loop is not predictable. It might be a case, when first element will be `VerificationRelationshipGeneral`. 
5. In this case function [verificationRelationshipName()](https://github.com/hyperledger/aries-framework-go/blob/50313f0971cff8b74e4ad0cb1ce45910f6653352/component/models/jwt/didsignjwt/signjwt.go#L246) returns `""`
6. Then, [condition](https://github.com/hyperledger/aries-framework-go/blob/main/component/models/dataintegrity/signer.go#L139C3-L141C4) 

```
if rel == "" {
			rel = "assertionMethod"
		}
````
takes place and declares hardcoded relationship.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-01 08:31:05 +0000 UTC
    </div>
</div>

