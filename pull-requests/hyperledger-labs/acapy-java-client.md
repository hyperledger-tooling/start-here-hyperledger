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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/4" class=".btn">#4</a>
            </td>
            <td>
                <b>
                    https://github.com/hyperledger-labs/acapy-java-client/issues/3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 15:54:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Feature/0.7.0 pre.3
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
        Created At 2021-06-25 13:03:51 +0000 UTC
    </div>
</div>

