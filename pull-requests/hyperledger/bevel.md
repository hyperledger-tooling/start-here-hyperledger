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
                PR <a href="https://github.com/hyperledger/bevel/pull/2079" class=".btn">#2079</a>
            </td>
            <td>
                <b>
                    [shared] cert-manager for TLS certificate creation using letsencrypt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Added Cert-manager helm chart
added configuration to install cert-manager helm chart, create letsencrypt clusterissuer and create tls certificate for Ambassador 
updated network.yaml/network-schema.json to have new field called fqdn, which would be needed for successful creation of tls  certificate, if fqdn is not provided , self signed certificate will be created as before

 

**Reviewed by**
@suvajit-sarkar @sownak @jagpreetsinghsasan 

 

**Linked issue**
#2036 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 06:13:37 +0000 UTC
    </div>
</div>

