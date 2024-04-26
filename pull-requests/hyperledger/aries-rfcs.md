---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    RFC 0809 - VCDI Credential offer request alternate proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'd like to suggest a re-alignment with the vc-api approach for the credential offer attachment. I'm not convinced the suggested change provides sufficient improvements and the rational aligns with the direction of the vc-api. The Credential Offer Exceptions section is in line with the recent discussions on the vc-api calls.

This change seems to get rid of a dedicated options field and put all options at the root layer of the request.

The JSON-LD attachment dates from 2021 and the vc-api specification has changed since then.

I have a few questions:

- Why include the data model version in the options? Could it not be derived from the context? In which scenario would an array be beneficial?
- Why include a `binding_required` bool? Could it not be assumed as required if there is a `binding_method` present? Is there a scenario where the binding isn't required but a method is provided?

@TimoGlastra 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 16:05:25 +0000 UTC
    </div>
</div>

