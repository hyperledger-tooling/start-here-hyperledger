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
                PR <a href="https://github.com/hyperledger/fabric/pull/2955" class=".btn">#2955</a>
            </td>
            <td>
                <b>
                    Refactor idemix implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the internal implementation of the idemix protocol and uses
an external dependency that contains the same implementation.

Signed-off-by: Alessandro Sorniotti <aso@zurich.ibm.com>

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The idemix is factored out of the repo and now imported as a dependency.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 15:58:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2954" class=".btn">#2954</a>
            </td>
            <td>
                <b>
                    Add OpenTelemetry tracing with grpc interceptors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- New feature

#### Description

Adds OpenTelemetry tracing by adding interceptors on all gRPC communications.

#### Related issues
This is tied to https://github.com/hyperledger/fabric-rfcs/blob/main/text/0000-opentelemetry-tracing.md

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 15:39:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2953" class=".btn">#2953</a>
            </td>
            <td>
                <b>
                    [Backport]  #2936  to release-2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #2936 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 15:04:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2952" class=".btn">#2952</a>
            </td>
            <td>
                <b>
                    Improve wording of log message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The log message that indicates which, if any, extra endorsers are required by the gateway is unclear.
This commit improves the wording.

Resolves https://github.com/hyperledger/fabric-gateway/issues/203

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 14:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2951" class=".btn">#2951</a>
            </td>
            <td>
                <b>
                    Randomize selection of orderer nodes with retry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the Submit() API method, the list of available orderers has been randomized to support improved load balancing.
Retry logic has been added such that if the selected orderer fails to return a success code, then the next orderer in the list is tried. If no orderers succeed, then return an error (containing details from each orderer) to the client.

Resolves #2912 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 09:42:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2950" class=".btn">#2950</a>
            </td>
            <td>
                <b>
                    Add Information about AWS HSM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change
- Documentation update

#### Description
Add AltId documentation for HSM


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 08:48:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2949" class=".btn">#2949</a>
            </td>
            <td>
                <b>
                    correct logger labels after cloning block puller.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jay Guo <guojiannan1101@gmail.com>

#### Type of change

- Bug fix

#### Description

When block puller is cloned for an application channel, its logger is inherited, with label of system channel name. This would be very confusing when reading logs. This PR fixes it by overriding logger with correct label.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 08:37:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2947" class=".btn">#2947</a>
            </td>
            <td>
                <b>
                    Improve an error message in `InstallChaincode`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds the package ID to the error message in the case of 'chaincode already successfully installed'.

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

In case a 'chaincode already successfully installed' error occurs when installing a chaincode, Fabric admins cannot to know the package ID. In this case, if multiple chaincode packages with the same label are installed, it is not possible to identify them later by using `queryinstalled`.

So, this patch adds the package ID to the error message in the case of 'chaincode already successfully installed'.

#### Additional details

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 07:40:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2945" class=".btn">#2945</a>
            </td>
            <td>
                <b>
                    [Release-2.2 BP FAB-2643]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a backport of pull request #2643

This backport required upgrading viper to `v1.1.1` as in the main branch, cherry-pick some related fixes to this upgrade. 

#1523  (only https://github.com/hyperledger/fabric/pull/1523/commits/7dee9f7f0403e4ce993a601a6cf2545a65ebbf0b "Use UnmarshalKey to retrieve peer BCCSP config" to fix pkcs11 suite)
#1511 (fully)

nothing new was added, just exact backport of #2643 with a bit of #1523 and full #1511
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-25 19:50:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2944" class=".btn">#2944</a>
            </td>
            <td>
                <b>
                    docs: Use html_style property instead of add_stylesheet()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add_stylesheet() is deprecated since Sphinx 1.8

Fix this build error on Sphinx 1.8 or higher

Exception occurred:
  File "docs/source/conf.py", line 137, in setup
    app.add_stylesheet('css/custom.css')
AttributeError: 'Sphinx' object has no attribute 'add_stylesheet'

Signed-off-by: Justin Yang <justin.yang@themedium.io>

#### Type of change
- Bug fix

#### Description
add_stylesheet() is deprecated since Sphinx 1.8 (https://www.sphinx-doc.org/en/master/extdev/appapi.html)

> Changed in version 1.8: Renamed from app.add_stylesheet(). And it allows keyword arguments as attributes of link tag.

Fix this build error on Sphinx 1.8 or higher
```
Exception occurred:
  File "docs/source/conf.py", line 137, in setup
    app.add_stylesheet('css/custom.css')
AttributeError: 'Sphinx' object has no attribute 'add_stylesheet'
```

The latest version is 4.2.0 now. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 00:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2943" class=".btn">#2943</a>
            </td>
            <td>
                <b>
                    docs: Don't apply the syntax highlighting of python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The syntax highlighting of pyhon is applied in the example
of read() and write() transactions.
For readability, don't apply the syntax highlighting.

Signed-off-by: Justin Yang <justin.yang@themedium.io>

#### Type of change
- Documentation update

#### Description
Fix the style of the example of transactions in [Read-Write set semantics](https://hyperledger-fabric.readthedocs.io/en/latest/readwrite.html) document for readability.
The fix makes showing them as just plain text.

The syntax highlighting of python has been applied in the below example.

> World state: (k1,1,v1), (k2,1,v2), (k3,1,v3), (k4,1,v4), (k5,1,v5)
> T1 -> Write(k1, v1'), Write(k2, v2')
> T2 -> Read(k1), Write(k3, v3')
> T3 -> Write(k2, v2'')
> T4 -> Write(k2, v2'''), read(k2)
> T5 -> Write(k6, v6'), read(k5)

The style of python string has been applied in ```'), Write(k2,v2'``` in T1', ```')``` in T2, `''` in T3, and
```
'''), read(k2)
T5 -> Write(k6, v6'), read(k5)
```
as multiline.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 15:03:17 +0000 UTC
    </div>
</div>

