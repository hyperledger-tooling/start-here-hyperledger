---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2281" class=".btn">#2281</a>
            </td>
            <td>
                <b>
                    [ci-skip] Upgrade Hashicorp Vault version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Update Hashicorp Vault version to 1.13.1. To carry out the tests, a vault has been deployed following the steps in this video. https://www.youtube.com/watch?v=eKMDgKshjQ8&list=PL0MZ85B_96CFJUzic2ZF9rposfx2hr2rm.
Using  version of helm search repo hashicorp/vault --versions.
![image](https://github.com/hyperledger/bevel/assets/83813093/ea76cc54-e256-4914-8f33-19c83c42131a)

Modifications
-------------
docs/source/faq.md
docs/source/prerequisites.md
platforms/shared/configuration/roles/setup/vault/defaults/main.yaml

Fixes
#2282

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 10:27:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2280" class=".btn">#2280</a>
            </td>
            <td>
                <b>
                    [ci-skip] enable cactus connector.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(quorum): enable Cactus connector for the GoQuorum platform**

```
This commit introduces the integration of the Cactus connector into the GoQuorum platform. Key highlights of this integration include:
 • Added Cactus connector to the Quorum platform
 • The connector promotes interoperability between different decentralized networks, furthering the growth and adoption of blockchain technology.
 • The integration improves the overall functionality of the system.
```

fixes #2253
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 12:28:38 +0000 UTC
    </div>
</div>

