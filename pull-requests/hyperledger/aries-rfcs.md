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
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    Add status STALLED and change status of many proposed RFCs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We have many RFCs that are in the "Proposed" status that are very unlikely to be progressed any further. To clear them out so that people have a better view of the active work in Aries, a new status "STALLED" has been added, and the status of many proposed RFCs have been changed to either STALLED, DEMONSTRATED or ACCEPTED, as appropriate based on the work done on the RFCs.

STALLED differs from the RETIRED state in that STALLED is direct from PROPOSED, whereas RETIRED is from a more advanced state, where implementation work was done, evaluated and found to be no longer of use.  STALLED just means that the idea never got beyond the idea stage.

Updated statuses:

-  STALLED:   concepts/0029-message-trust-contexts/README.md
-  RETIRED:   concepts/0051-dkms/README.md
-  STALLED:   concepts/0207-credential-fraud-threat-model/README.md
-  STALLED:   concepts/0217-linkable-message-paths/README.md
-  STALLED:   concepts/0250-rich-schemas/README.md
-  STALLED:   concepts/0257-private-credential-issuance/README.md
-  STALLED:   concepts/0268-unified-didcomm-agent-deeplinking/README.md
-  STALLED:   concepts/0289-toip-stack/README.md
-  STALLED:   concepts/0420-rich-schemas-common/README.md
-  STALLED:   concepts/0478-coprotocols/README.md
-  STALLED:   concepts/0700-oob-through-redirect/README.md
-  STALLED:   features/0024-didcomm-over-xmpp/README.md
-  STALLED:   features/0030-sync-connection/README.md
-  STALLED:   features/0075-payment-decorators/README.md
-  STALLED:   features/0114-predefined-identities/README.md
-  STALLED:   features/0116-evidence-exchange/README.md
-  STALLED:   features/0193-coin-flip/README.md
-  STALLED:   features/0213-transfer-policy/README.md
-  STALLED:   features/0214-help-me-discover/README.md
-  STALLED:   features/0249-rich-schema-contexts/README.md
-  STALLED:   features/0281-rich-schemas/README.md
-  STALLED:   features/0309-didauthz/README.md
-  STALLED:   features/0327-crypto-service/README.md
-  STALLED:   features/0334-jwe-envelope/README.md
-  STALLED:   features/0335-http-over-didcomm/README.md
-  STALLED:   features/0347-proof-negotiation/README.md
-  STALLED:   features/0351-purpose-decorator/README.md
-  STALLED:   features/0418-rich-schema-encoding/README.md
-  STALLED:   features/0428-prepare-issue-rich-credential/README.md
-  STALLED:   features/0429-prepare-req-rich-pres/README.md
-  STALLED:   features/0445-rich-schema-mapping/README.md
-  STALLED:   features/0446-rich-schema-cred-def/README.md
-  STALLED:   features/0482-coprotocol-protocol/README.md
-  STALLED:   features/0641-linking-binary-objects-to-credentials/README.md
-  STALLED:   features/0693-credential-representation/README.md
-  DEMONSTRATED:   features/0755-oca-for-aries/README.md
-  DEMONSTRATED:   features/0756-oca-for-aries-style-guide/README.md
-  DEMONSTRATED:   features/0780-data-urls-images/README.md
-  ACCEPTED:   features/0794-did-rotate/README.md
-  DEMONSTRATED:   features/0804-didcomm-rpc/README.md
-  DEMONSTRATED:   features/0809-w3c-data-integrity-credential-attachment/README.md


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 14:02:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    Cleanup RFCs for mkdocs website generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The vast majority of the changes are just to add "mailto:" to the front of the email addresses in the RFCs -- that was missed in the templates, and it carried into the RFCs themselves.

A few other cleanups of paths, and tweaks to the generator.  In the process, a couple of clarifications were made -- minor, to do with things that have changed over time.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-30 19:47:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/824" class=".btn">#824</a>
            </td>
            <td>
                <b>
                    Tweak to the GitHub Action for deploying the docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - **First draft of the Aries RFCs website -- generation and publishing**
- **Tweak to the GitHub Action for deploying the docs**

Almost got it right. Just a tweak needed...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-27 23:45:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/823" class=".btn">#823</a>
            </td>
            <td>
                <b>
                    First draft of the Aries RFCs website -- generation and publishing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A PR that might trigger the publication of a GH Pages site - depending on the success of the included GHAction. I tested it as much as I could.

In theory, this should create a gh-pages branch from which we can publish the site. The gh-pages static content will be based on the docs generated by the GHAction. From there we can publish it.

As noted on the Aries Working Group call (20240327) this is the start of the work on this, there are some todos that will be added as issues to be worked on.

This should be a "do no harm" PR -- it shouldn't affect anything other than adding a gh-pages branch in the repo.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-27 23:26:59 +0000 UTC
    </div>
</div>

