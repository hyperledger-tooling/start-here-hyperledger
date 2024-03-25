---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    Update the versions of fabric sdks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This rationalises the versions and we should only document the following binding versions

1, 1.4 (use 1.4 legacy sdk)
2.2 (use 2.2 legacy sdk)
2.4, 2.5, 3, fabric-gateway (use the fabric-gateway sdk)

We will keep 2.4 (for legacy reasons only as 2.4 was never LTS), 2.5 to cover the published versions of fabric we support however the binding of fabric-gateway should be the one going forward and seen in the documentation.
because Fabric 2 changed the recommended client version in a point release (2.5 deprecated the legacy sdks and the only real option if the fabric-gateway) otherwise we will specify a single digit version for fabric (1,3)

the 1.4, 2.2 sdks are now deprecated and 2.2 is now or version soon to be out of lts, therefore fabric-gateway is the only version that will and should be used in the future and there is no plan to change the client side much given the reduction in resource of people using it and the use of SmartBFT should not affect the client side version (I hope :-) )



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-25 10:53:35 +0000 UTC
    </div>
</div>

