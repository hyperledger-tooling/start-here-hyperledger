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
                PR <a href="https://github.com/hyperledger/bevel/pull/2308" class=".btn">#2308</a>
            </td>
            <td>
                <b>
                    [ci-skip] Update HAProxy port to 443 and related hlf changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update HA Proxy port to 443 and remove all reference to 8443 from Fabric
Also includes merge from main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 12:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2307" class=".btn">#2307</a>
            </td>
            <td>
                <b>
                    [ci-skip] generate storage class through a single template file.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**feat(shared): dynamically generate storage class through a single template file for various cloud providers**

This commit introduces a solution to simplify the process of generating storage classes for various cloud providers in the bevel project.

**Changes**:
- Created Helm chart `storage_class` with a single template file for dynamic generation of storage classes based on various cloud providers.
- Implemented Helm Release (HR) template file to configure the `storage_class` chart.

 
**Additional changes**:
- Fixed code to generate the StorageClass HR file inside the organization directory, ensuring proper deletion during network reset.
- Fixed deletion code to effectively remove deployed StorageClasses from the Kubernetes cluster.

**Benefits**:
- Simplifies switching between cloud providers by updating the `cloud_provider`field in the network configuration file.
- Streamlines the generation and management of storage classes in the bevel project.
- Reduces code duplication and maintenance overhead by utilizing a single template file for all cloud providers.

fixes #2306
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 13:23:14 +0000 UTC
    </div>
</div>

