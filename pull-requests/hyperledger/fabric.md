---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3686" class=".btn">#3686</a>
            </td>
            <td>
                <b>
                    Use safe accessors for RWset protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the Getter functions rather than direct access to fields in the proto structures.

Resolves #3685 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-13 08:40:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3681" class=".btn">#3681</a>
            </td>
            <td>
                <b>
                    Use env variables to initialize the PKCS11 BCCSP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The environment variables to configure the PKCS11 BCCSP are ignored for the peer node, such as CORE_PEER_BCCSP_PKCS11_LIBRARY. This change allows specifying the BCCSP Default and to configure all of the PKCS11 BCCSP settings using environment variables.

Signed-off-by: Jonathan Patchell <Jonathan.Patchell@thalesgroup.com>

#### Type of change

- Bug fix

#### Description

When integrating the peer node with an HSM, it isn't possible to specify environment variables to configure the PKCS11 BCCSP. With these changes the environment variables are no longer ignored allowing configuration from environment variables for the  PKCS11 BCCSP.

#### Additional details

#### Related issues

#1900

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 19:46:34 +0000 UTC
    </div>
</div>

