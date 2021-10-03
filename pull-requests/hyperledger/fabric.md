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
                PR <a href="https://github.com/hyperledger/fabric/pull/2968" class=".btn">#2968</a>
            </td>
            <td>
                <b>
                    Evaluate() error response for node chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The gateway Evaluate() method is not returning the error response to the client for node chaincodes. The code path for node chaincode errors is different than for Go chaincodes (this is a known separate issue).
It turns out the endorser is handling this difference and populates the Response field of the ProposalResponse accordingly.  The gateway needs to use this field rather than the one in the ChaincodeAction structure.

Resolves https://github.com/hyperledger/fabric-gateway/issues/193

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 15:54:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2967" class=".btn">#2967</a>
            </td>
            <td>
                <b>
                    Rename persistent_msgs to persistance to avoid protobuf conflict
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Due to two protobuf files having the same name, when they are registered twice, a panic occurs.


`git diff` between the old pb.go and the new pb.go yields:
```


2c2
< // source: persistent_msgs.proto
---
> // source: persistance.proto
34c34
< 	return fileDescriptor_0f0cbd2d16bac879, []int{0}
---
> 	return fileDescriptor_a374ca4de69122a4, []int{0}
66c66
< func init() { proto.RegisterFile("persistent_msgs.proto", fileDescriptor_0f0cbd2d16bac879) }
---
> func init() { proto.RegisterFile("persistance.proto", fileDescriptor_a374ca4de69122a4) }
68,69c68,69
< var fileDescriptor_0f0cbd2d16bac879 = []byte{
< 	// 149 bytes of a gzipped FileDescriptorProto
---
> var fileDescriptor_a374ca4de69122a4 = []byte{
> 	// 145 bytes of a gzipped FileDescriptorProto
71,79c71,79
< 	0x10, 0x06, 0x60, 0x44, 0x11, 0xec, 0xe0, 0x50, 0x10, 0x3a, 0x8a, 0x93, 0x53, 0x83, 0xf4, 0x0d,
< 	0xc4, 0xd1, 0x41, 0x74, 0x73, 0x91, 0x26, 0xfd, 0x4d, 0x0f, 0xd2, 0x5c, 0xb8, 0x3b, 0x07, 0xdf,
< 	0x5e, 0xe8, 0xe6, 0xf6, 0x6d, 0x5f, 0xb5, 0x2b, 0x10, 0x25, 0x35, 0x64, 0x7b, 0x4d, 0x1a, 0xb5,
< 	0x2d, 0xc2, 0xc6, 0xf5, 0xd6, 0xa4, 0xcf, 0x4a, 0xc8, 0xa6, 0xc6, 0x82, 0x43, 0x5b, 0x35, 0x37,
< 	0xe4, 0x81, 0x72, 0xbc, 0x20, 0xc1, 0xf0, 0x30, 0x96, 0x3e, 0xe2, 0x4a, 0x6a, 0x75, 0x5d, 0xad,
< 	0x12, 0xa9, 0x35, 0x8b, 0xfd, 0xf2, 0xb8, 0xb9, 0xcf, 0x3e, 0x77, 0xcf, 0x53, 0x24, 0x1b, 0x3f,
< 	0xbe, 0x0d, 0x3c, 0xb9, 0xf1, 0x5b, 0x20, 0x09, 0x43, 0x84, 0xb8, 0x77, 0xef, 0x85, 0x82, 0x0b,
< 	0x2c, 0x70, 0xff, 0x89, 0x5f, 0xcf, 0x77, 0xf7, 0x0b, 0x00, 0x00, 0xff, 0xff, 0xf5, 0x44, 0x88,
< 	0x95, 0x94, 0x00, 0x00, 0x00,
---
> 	0x10, 0x06, 0x60, 0x44, 0x11, 0xec, 0x20, 0xd8, 0xa9, 0xa3, 0x38, 0x39, 0x35, 0x48, 0xdf, 0x40,
> 	0x1c, 0x1d, 0x44, 0x37, 0xb7, 0x24, 0xfd, 0x4d, 0x0f, 0x62, 0x2e, 0xdc, 0x9d, 0x83, 0x6f, 0x2f,
> 	0x74, 0x73, 0xfb, 0xb6, 0xaf, 0xd9, 0x55, 0x88, 0x92, 0x9a, 0x2f, 0x11, 0x7d, 0x15, 0x36, 0x6e,
> 	0xb7, 0x26, 0xbe, 0x28, 0xa1, 0x98, 0x1a, 0x0b, 0x0e, 0x7d, 0xd3, 0xdd, 0x50, 0x46, 0x2a, 0xe9,
> 	0x82, 0x0c, 0xc3, 0xc3, 0x58, 0x7c, 0xc2, 0x95, 0xd4, 0xda, 0xb6, 0x59, 0x65, 0x52, 0xeb, 0x16,
> 	0xfb, 0xe5, 0x71, 0x73, 0x9f, 0x7d, 0x1e, 0x9e, 0xa7, 0x44, 0x36, 0x7d, 0x42, 0x1f, 0xf9, 0xed,
> 	0xa6, 0x6f, 0x85, 0x64, 0x8c, 0x09, 0xe2, 0x5e, 0x3e, 0x08, 0x45, 0x17, 0x59, 0xe0, 0xfe, 0x93,
> 	0xb0, 0x9e, 0xef, 0xe1, 0x17, 0x00, 0x00, 0xff, 0xff, 0xa1, 0xb1, 0xe2, 0x32, 0x90, 0x00, 0x00,
> 	0x00,


```

Change-Id: If27e6b3a7c063661411dcc7cebe14b2393f7d28f
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 14:40:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2966" class=".btn">#2966</a>
            </td>
            <td>
                <b>
                    Sort chaincode interests in tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alessandro Sorniotti <aso@zurich.ibm.com>

#### Type of change

- Bug fix

#### Description

Endorser tests suffer accidental failures due to non-deterministic map traversal. The PR fixes that by sorting results before asserting their content.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 13:16:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2965" class=".btn">#2965</a>
            </td>
            <td>
                <b>
                    Fix the project status to 'Graduated' instead of 'Active'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch fixes the project status to 'Graduated' in some docs, instead of 'Active' as the former name.
Also, this update the link to the Hyperledger Lifecycle document to the new location.

#### Type of change

- Bug fix
- Documentation update

#### Description

This patch fixes the project status to 'Graduated' in some docs, instead of 'Active' as the former name.
Also, this update the link to the Hyperledger Lifecycle document to the new location.

#### Additional details


#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 02:44:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2964" class=".btn">#2964</a>
            </td>
            <td>
                <b>
                    [Backport] #2936 to release-1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">needs-release-note</span>
            </td>
            <td>
                Backport of #2936
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 16:50:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2963" class=".btn">#2963</a>
            </td>
            <td>
                <b>
                    Improve error messages when no endorsers found
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Clarify the wording in the error message returned from gateway Submit() when no endorsement plan can be created.

Add the chaincode name to the error message returned from Evaluate() when no endorsing peer can be found for the chaincode/channel combination.

Resolves https://github.com/hyperledger/fabric-gateway/issues/199

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 15:32:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2962" class=".btn">#2962</a>
            </td>
            <td>
                <b>
                    Add Information about AWS HSM (backport #2950)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2950 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 11:46:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2961" class=".btn">#2961</a>
            </td>
            <td>
                <b>
                    Add Information about AWS HSM (backport #2950)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2950 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 11:46:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2959" class=".btn">#2959</a>
            </td>
            <td>
                <b>
                    Backport setEvent information to 2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #2958
Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change
- Documentation update

#### Description
backport setEvent information to 2.2


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 09:21:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2957" class=".btn">#2957</a>
            </td>
            <td>
                <b>
                    docs: Add the path of softhsm2.conf for macOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Yang <justin.yang@themedium.io>

#### Type of change
- Documentation update

#### Description
There are no ```softhsm``` directory and ```softhsm2.conf``` file under ```/etc/``` for macOS.
There is ```softhsm2.conf``` file under ```/usr/local/etc/softhsm/``` by brew installation.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 07:38:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2956" class=".btn">#2956</a>
            </td>
            <td>
                <b>
                    Update links for Jira to GitHub issue transition in README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update links for Jira to GitHub issue transition in README

#### Type of change

- Documentation update

#### Description

This patch updates links for Jira to GitHub issue transition in README.

#### Additional details

Related PR:
- https://github.com/hyperledger/fabric/pull/2907

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 02:40:41 +0000 UTC
    </div>
</div>

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
                <span class="chip">needs-release-note</span>
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

