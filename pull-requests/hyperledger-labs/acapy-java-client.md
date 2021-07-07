---
layout: default
title: acapy-java-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/acapy-java-client
---

# acapy-java-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/acapy-java-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    extend presentproofrequest-restrictions-for-generic-restrictions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added support for generic restrictions in PresentProofRequest. Added addAttributeValueRestriction for convenience to the ProofRestrictionsBuilder.

Signed-off-by: Lars Wegner <lars.wegner2@de.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 15:34:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/7" class=".btn">#7</a>
            </td>
            <td>
                <b>
                    Extend present proof request builder with lombok.singular
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @lombok.Singular is needed to map ProofTemplates to PresentProofRequest efficiently.

The major change is, that the fields PresentProofRequest#requestedPredicates and PresentProofRequest#requestedAttributes now have a java.util.HashMap instead of a java.util.LinkedHashMap when PresentProofRequestBuilder is used.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 11:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/6" class=".btn">#6</a>
            </td>
            <td>
                <b>
                    Add a method to get all schemas from Aries Cloudagent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the second approach to propose a method to get all Schema Ids from the Aries Cloudagent. Corrections include a filter as suggested and a simple unit test.

Signed-off-by: Stefan Hauffe <stefan.hauffe@mgm-tp.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 06:55:59 +0000 UTC
    </div>
</div>

