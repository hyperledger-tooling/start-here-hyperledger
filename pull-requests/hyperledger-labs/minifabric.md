---
layout: default
title: minifabric
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minifabric
---

# minifabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minifabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    Allows setting the CA admin passwd using spec.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The admin CA password is hardcoded in config_apply.yaml, this PR enables the use of adminPassword if it is defined in spec.yml. 

`# spec.yaml 
fabric:
  cas:
  - "ca1.devops.io"
  peers: 
  - "peer1.devops.io"
  orderers:
  - "orderer1.devops-orderer.io"
  settings:
    ca:
      FABRIC_LOGGING_SPEC: DEBUG
     adminPassword: "test"
    peer:
      FABRIC_LOGGING_SPEC: DEBUG
    orderer:
      FABRIC_LOGGING_SPEC: DEBUG
`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-26 16:34:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minifabric/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    fix cergen for subjectAltName
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #274
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 03:37:31 +0000 UTC
    </div>
</div>

