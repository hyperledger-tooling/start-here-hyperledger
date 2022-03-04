---
layout: default
title: indy-did-method
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-did-method
---

# indy-did-method <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-did-method){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    docs: remove DIDDoc validation requiring current DID Core JSON-LD context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is the product of the discussion in Issue #57. This DID Core context validation does not ensure that the resulting JSON-LD DIDDoc is valid and it would need to be updated if the DID Core context is changed. It is the responsibility of the content creator to validate that the resulting DIDDoc is valid JSON-LD. 

Signed-off-by: Char Howland <char@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 05:57:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Fix/52 option2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Attempt to resolve #39 and #52 

While making the changes, I felt like Option 2 is reasonably clear and makes sense because in both cases accumulator values and (in the case of `GET_REVOC_REG_DELTA`) indices are returned. So it's arguably the same ledger object.

But I'm open to providing an additional PR for Option 1.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 08:07:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Create resolvable json-ld for DID Doc examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The main focus was to try to create fully resolvable json-ld and updating to be compliant to the examples given in did-core 
Fixes #51

Signed-off-by: Christian Bormann <ChristianCarl.Bormann@de.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 15:55:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Add version to document -- fixes #37
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 12:30:58 +0000 UTC
    </div>
</div>

