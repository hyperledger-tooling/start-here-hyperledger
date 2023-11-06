---
layout: default
title: open-enterprise-agent
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/open-enterprise-agent
---

# open-enterprise-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/open-enterprise-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Open Enterprise Agent v1.18.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    prism-agent-v1.18.0
                </span>
            </td>
            <td>
                ## What's Changed
* test: multitenancy tests update by @antonbaliasnikov in https://github.com/hyperledger-labs/open-enterprise-agent/pull/723
* test: fix e2e test correctly initializing multitenancy by @antonbaliasnikov in https://github.com/hyperledger-labs/open-enterprise-agent/pull/724
* fix: correct typo on sts header (dmax -> max) by @davidpoltorak-io in https://github.com/hyperledger-labs/open-enterprise-agent/pull/726
* fix(prism-agent): introduce generic secret store for CD by @patlo-iog in https://github.com/hyperledger-labs/open-enterprise-agent/pull/727
* fix: Adding localhost environment variable in run.sh script for local development by @elribonazo in https://github.com/hyperledger-labs/open-enterprise-agent/pull/728
* fix: Separate config for integration flow ATL-5777 by @milosbackonja in https://github.com/hyperledger-labs/open-enterprise-agent/pull/731
* fix: Separate config for integration flow ATL-5777 by @milosbackonja in https://github.com/hyperledger-labs/open-enterprise-agent/pull/733
* fix: Integration flow by @milosbackonja in https://github.com/hyperledger-labs/open-enterprise-agent/pull/734
* fix: Renaming values.yml [skip ci] ATL-5777  by @milosbackonja in https://github.com/hyperledger-labs/open-enterprise-agent/pull/735
* fix: Changing yq command [skip ci] ATL-5777 by @milosbackonja in https://github.com/hyperledger-labs/open-enterprise-agent/pull/736
* fix: Adding labels [skip ci] by @milosbackonja in https://github.com/hyperledger-labs/open-enterprise-agent/pull/737
* fix: Integration flow ATL-5777 by @milosbackonja in https://github.com/hyperledger-labs/open-enterprise-agent/pull/738
* fix: upgrade vault and quill versions by @patlo-iog in https://github.com/hyperledger-labs/open-enterprise-agent/pull/739
* docs: add ADR on keycloak authorisation service for multitenancy [skip ci] by @patlo-iog in https://github.com/hyperledger-labs/open-enterprise-agent/pull/730
* fix(prism-agent): check issuing DID validity when creating a VC offer by @bvoiturier in https://github.com/hyperledger-labs/open-enterprise-agent/pull/740
* refactor: update zio-http to 3.0.0-RC2 and tapir to 1.6.4, remove legacy tapir by @shotexa in https://github.com/hyperledger-labs/open-enterprise-agent/pull/729
* fix: prohibit tenants to use equal api keys by @yshyn-iohk in https://github.com/hyperledger-labs/open-enterprise-agent/pull/742
* build: add local developement keycloak and init script by @patlo-iog in https://github.com/hyperledger-labs/open-enterprise-agent/pull/743
* fix: change repository and name for rest api clients by @antonbaliasnikov in https://github.com/hyperledger-labs/open-enterprise-agent/pull/745
* fix(prism-agent): configure APISIX to return CORS headers from Prism Agent endpoints by @bvoiturier in https://github.com/hyperledger-labs/open-enterprise-agent/pull/746
* feat(prism-agent): implement AnonCreds issuance flow by @FabioPinheiro in https://github.com/hyperledger-labs/open-enterprise-agent/pull/693
* fix(prism-agent): fix docker env variables interpolation issue by @bvoiturier in https://github.com/hyperledger-labs/open-enterprise-agent/pull/751
* fix: improve performance for background jobs in multitenancy mode by @mineme0110 in https://github.com/hyperledger-labs/open-enterprise-agent/pull/749
* fix(prism-agent): return relevant errors on offer creation by @bvoiturier in https://github.com/hyperledger-labs/open-enterprise-agent/pull/754
* fix(prism-agent): agent should read DIDComm port from config by @bvoiturier in https://github.com/hyperledger-labs/open-enterprise-agent/pull/757
* chore: fix npm client publishing repo by @antonbaliasnikov in https://github.com/hyperledger-labs/open-enterprise-agent/pull/760
* feat(prism-agent): add keycloak authorization support to endpoints by @patlo-iog in https://github.com/hyperledger-labs/open-enterprise-agent/pull/753
* feat: add new auth params by @womfoo in https://github.com/hyperledger-labs/open-enterprise-agent/pull/762
* docs: replace broken link in Issue.md, AnonCreds Credential definition by @elribonazo in https://github.com/hyperledger-labs/open-enterprise-agent/pull/763
* docs: fix typo in docs link by @elribonazo in https://github.com/hyperledger-labs/open-enterprise-agent/pull/764
* feat: disable cors by default by @davidpoltorak-io in https://github.com/hyperledger-labs/open-enterprise-agent/pull/747
* fix:  all performance tests run succesfully, add group thresholds by @davidpoltorak-io in https://github.com/hyperledger-labs/open-enterprise-agent/pull/750
* feat:  presentation API refactor by @CryptoKnightIOG in https://github.com/hyperledger-labs/open-enterprise-agent/pull/765
* feat: migrate docker image of the agent to Java 21 by @yshyn-iohk in https://github.com/hyperledger-labs/open-enterprise-agent/pull/758
* ci: fix client generation by @amagyar-iohk in https://github.com/hyperledger-labs/open-enterprise-agent/pull/766


**Full Changelog**: https://github.com/hyperledger-labs/open-enterprise-agent/compare/prism-agent-v1.16.0...prism-agent-v1.18.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/open-enterprise-agent/releases/tag/prism-agent-v1.18.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-24 11:08:16 +0000 UTC
    </span>
</div>

