---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.2.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 18:30:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/293" class=".btn">#293</a>
            </td>
            <td>
                <b>
                    Make idemix use Mathlib instead of AMCL directly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit makes Fabric-CA use Mathlib instead of AMCL.
Mathlib supports several curves, and they can now be configured by setting:
- idemix.curve' key in the server config file
 - 'idemix.curve' key in the client config file
- --idemix.curve flag when running the fabric-ca-client binary
- --idemix.curve flag when running the fabric-ca-server binary

  
    
The possible values for curve identifiers are: 'amcl.Fp256bn', 'gurvy.Bn254', 'amcl.Fp256Miraclbn'
    
If not specified, it fallbacks to the first one in the list
    
More details on the rational can be found in https://github.com/hyperledger/fabric-ca/issues/292


Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 07:46:12 +0000 UTC
    </div>
</div>

