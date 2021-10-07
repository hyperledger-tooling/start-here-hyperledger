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
                PR <a href="https://github.com/hyperledger/fabric/pull/2973" class=".btn">#2973</a>
            </td>
            <td>
                <b>
                    Add clarifications to dev env versions in doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update Go version and add caveats to dev env version doc.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 22:11:57 +0000 UTC
    </div>
</div>

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

