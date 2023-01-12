---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Integration test overhaul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR to resolve issues with the integration tests failing; slightly larger PR than ideal for the scale of the fix. However the original infrastructure used for the integration tests was a derivative of the (very) old byfn test network - and it was using old lifecycle and not updated in any recent time.

Therefore it seemed a manageable risk to remove it entirely and go with the modern solution of pulling in the single docker image of Microfab to use to spin up a real fabric network for testing. 

- additional tests are done with other deployments of Fabric in the fabric-tests repo
- microfab has all the features needed to support the 'integration/fv' testing of the chaincode, and is in one container

**Changes made:**
- Strand up Microfab rather than the multiple images
- Use a standard two org network as before (one peer per org so simpler than previously)
- The chaincode is built into a local repo inside each chaincode for testing
- The same tests are present with the same structure, minor changes made to support a slightly different approach 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 12:10:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    Update to fixed level of dependency checker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 09:12:26 +0000 UTC
    </div>
</div>

