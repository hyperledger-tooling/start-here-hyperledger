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
                PR <a href="https://github.com/hyperledger/bevel/pull/2338" class=".btn">#2338</a>
            </td>
            <td>
                <b>
                    [docs] Fix Sphinx version to solve build error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix Sphinx build errors on readthedocs

#2337
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 10:42:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2336" class=".btn">#2336</a>
            </td>
            <td>
                <b>
                    [ci-skip] Updated docs for minikube
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - updated docs for minikube
- MacOS tested with HyperKit as VirtualBox has issues
- Removed "GIT_RESET_PATH" as it slows down minikube deployment
Solves #2337
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 17:02:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2335" class=".btn">#2335</a>
            </td>
            <td>
                <b>
                    [ci-skip] remove support of molecule testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(shared): remove support of molecule testing

molecule test support were removed from all the platforms

fixes: #2331
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 13:37:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2333" class=".btn">#2333</a>
            </td>
            <td>
                <b>
                    [ci-skip] corrected missing variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Changes
- code indentation
- roadmap docs
## Fixes
- missing variable in playbooks calling sc and vault k8s creation 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 05:59:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2329" class=".btn">#2329</a>
            </td>
            <td>
                <b>
                    [ci-skip] enable prometheus for besu node metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(besu): enable prometheus for besu node metrics 

prometheus server deployments for individual organizations

fixes #2290
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 09:47:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2324" class=".btn">#2324</a>
            </td>
            <td>
                <b>
                    [ci-skip] Add README.md files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
Add readme files for all charts
Update the values.yaml files
Update the version in chart.yaml file

Modifications in charts
---------------------
platforms/r3-corda-ent/charts/auth
platforms/r3-corda-ent/charts/bridge
platforms/r3-corda-ent/charts/float
platforms/r3-corda-ent/charts/gateway
platforms/r3-corda-ent/charts/generate-pki-node
platforms/r3-corda-ent/charts/generate-pki
platforms/r3-corda-ent/charts/h2
platforms/r3-corda-ent/charts/idman
platforms/r3-corda-ent/charts/nmap
platforms/r3-corda-ent/charts/node-initial-registration 
platforms/r3-corda-ent/charts/node
platforms/r3-corda-ent/charts/notary-initial-registration 
platforms/r3-corda-ent/charts/notary
platforms/r3-corda-ent/charts/signer
platforms/r3-corda-ent/charts/zone

Fixes #2284
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 09:15:15 +0000 UTC
    </div>
</div>

