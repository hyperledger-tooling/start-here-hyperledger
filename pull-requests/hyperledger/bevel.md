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
                PR <a href="https://github.com/hyperledger/bevel/pull/2152" class=".btn">#2152</a>
            </td>
            <td>
                <b>
                    [fabric] Fix vault-auth when restart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- remove reviewer token in Vault_Kubernetes chart
- Add vault-auth as system:auth-delegator
- Add checks for certificate creation so that job checks are not carried again (jobs vanish when cluster restarts)
- Remove unnecessary fields from network.yaml samples for raft consensus

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 12:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2150" class=".btn">#2150</a>
            </td>
            <td>
                <b>
                    [besu]cert-manager setup for besu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**

As of now this is valid only for besu network

added the cert manager helm chart
added new filed in network-besu.yaml "issuer: default/letsencrypt"
updated the code to deploy the cert manager and install certificates using cert-manager using letsencrypt CA, this will run only if "issuer: letsencrypt" in network-besu.yaml, else self signed certs will be created as earlier
updated the reset-network.yaml file to delete the certs at the time of network deletion


 

**Reviewed by**
@sownak @suvajit-sarkar @jagpreetsinghsasan 

 

**Linked issue**
#2036 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 08:58:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2148" class=".btn">#2148</a>
            </td>
            <td>
                <b>
                    [ci-skip] workflow for alpine1.1 image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: RaviKiranJanjanam <ravi.kiran.janjanam@accenture.com>

**Changelog**

Added the workflow for alpine-image:1.1
fixed the repository name to be in lowercase for below files under workflow

.github/workflows/corda_images_build.yml
.github/workflows/docker_build.yml
.github/workflows/indy_image_build.yaml
.github/workflows/quorum_images_build.yml

 

**Reviewed by**
@sownak @suvajit-sarkar @jagpreetsinghsasan 

 

**Linked issue**
#2147 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 11:12:49 +0000 UTC
    </div>
</div>

