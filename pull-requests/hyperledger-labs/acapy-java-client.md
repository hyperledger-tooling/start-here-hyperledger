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
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    addition to proof parser
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
        Created At 2022-10-05 13:22:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/acapy-java-client/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    aggregated view for proof presentations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added an extractor class `RequestedProofParser` that is exposed via `PresentationExchangeRecord.collectAll()` that aggregates all: revealed attributes, revealed attribute groups, predicates, unrevealed attributes and self attested attributes into one simple view that can be mapped to the presentation request via its key. This is mainly for convenience reasons, as each group requires a slightly different handling. Existing extractor methods now also support self attested attributes.

 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 14:33:40 +0000 UTC
    </div>
</div>

