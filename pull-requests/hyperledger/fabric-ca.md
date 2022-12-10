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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    Publish release artifacts to conventional installation paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Bug fix

#### Description

This PR publishes the v1.5.6-beta release artifacts to GH as artifacts, stripping the semrev 'v' character for alignment with the traditional install-fabric.sh scripts. 

#### Additional details

#### Related issues

#### Release Note

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 18:37:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    Add some debug information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The cert file *must be* `cert.pem`; which in my case it wasn't.  Would have been nice to have some flexibility, however the error messages appeared to be suggestion idemix was an issue, and gave little clue as to what was wrong. 

- update the error message to give more indication of the file that should be checked
- Prevented idemix error from hiding x509

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-03 09:06:09 +0000 UTC
    </div>
</div>

