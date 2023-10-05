---
layout: default
title: iroha-2-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-2-docs
---

# iroha-2-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-2-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/417" class=".btn">#417</a>
            </td>
            <td>
                <b>
                    [docs] #414: move API specification to the docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">iroha2</span>
            </td>
            <td>
                Closes #414

---

Source: https://github.com/hyperledger/iroha/blob/39b1ca1e6887a463d7f5fd8c45c83bb697ee8ea6/docs/source/references/api_spec.md

Changes:

- Fixed mentions of structures in requests/responses, linked them to the data-model page
- Changed structure & formatting of the document
- Put TODOs for future

If you have a better idea of how this page might look like, you are very welcome!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 07:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/416" class=".btn">#416</a>
            </td>
            <td>
                <b>
                    'Security' section with all topics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">iroha2</span>
            </td>
            <td>
                Main differences from the last PR #374:
- Rearrangements:
   - **Keys for Network Deployment**: **Keys on the Client Side** subtopic moved to the **Public Key Cryptography** topic.
   - The rest of the **Keys for Network Deployment** topic moved back to the **Configuration and Management** section.
- **Security** header topic (`nav-security.md`) with overview and navigation added.
- **Password Security** topic (`password-security.md`) added.
- Additions and edits to the **Operational Security** topic (mostly based on comments by @appetrosyan in my last PR #374).
- Fixed formatting in some instances.
- Fixed dead links, added new internal links and links to outside sources.
- Added **Security** section and its topics to the `config.mts` file.
- Changes throughout the rest of the existing documentation to accommodate for removed links to topics that no longer exist.
- Occasional wording changes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 18:16:14 +0000 UTC
    </div>
</div>

