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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1259" class=".btn">#1259</a>
            </td>
            <td>
                <b>
                    fix: credentials must specify additional types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While writing test for AATH I noticed in the vc-data-model section on [types](https://www.w3.org/TR/vc-data-model/#types), the following excerpt:

> All credentials, presentations, and encapsulated objects MUST specify, or be associated with, additional more narrow types (like UniversityDegreeCredential, for example) so software systems can process this additional information.

This is also tested in the vc-test-suite: https://github.com/w3c/vc-test-suite/blob/gh-pages/test/vc-data-model-1.0/10-basic.js#L95-L99

This PR adds this restriction to the validation of VCs in ACA-Py
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 16:15:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1252" class=".btn">#1252</a>
            </td>
            <td>
                <b>
                    fix: check for expanded types in context checker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The checker method that checks for properties without a context was giving incorrect results for the vaccination context. This PR also checks if compaction expands a property as described in https://github.com/w3c-ccg/vaccination-vocab/issues/22


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-20 14:37:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1250" class=".btn">#1250</a>
            </td>
            <td>
                <b>
                    DIF PE - VCHolder backend-specific tag_query building and handle no given_id credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Addresses the following from #1247, @andrewwhitehead will this meet the requirement? 
> As discussed, I think this tag filtering belongs in VCHolder so that it can be specialized for the specific backends, but it's fine to merge this as-is and I can revisit it later with the shared-components work. Most important is that it works for now.
- resolve #1253
- Verification mechanism to check if the received presentation matches against the `constraints` in `presentation_definition`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-19 21:03:45 +0000 UTC
    </div>
</div>

