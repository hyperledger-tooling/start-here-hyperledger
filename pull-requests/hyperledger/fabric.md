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
                PR <a href="https://github.com/hyperledger/fabric/pull/4473" class=".btn">#4473</a>
            </td>
            <td>
                <b>
                    remove an unused parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

This commit removes an unused parameter named "namespace" from a function that computes the expiring block number for a private key stored in a collection with a "block to live" policy.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 12:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4472" class=".btn">#4472</a>
            </td>
            <td>
                <b>
                    Add inspect option into checkcommitreadiness command to output discre…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds `inspect` option into checkcommitreadiness command to output discrepancy details.

#### Type of change

- New feature

#### Description
I have proposed an extension to lifecycle chaincode checkcommitreadiness to provide details of the discrepancies as shown in  https://github.com/hyperledger/fabric/issues/4428.

As a sub-task stemming from issue #4428, this patch adds `inspect` option into checkcommitreadiness command to output discrepancy details.

After this patch is merged, I will submit some patches for the integration tests and documentation.

#### Additional details

The example of output when executing checkcommitreadiness with inspect flag in the implementation:

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect
Chaincode definition for chaincode 'basic', version '2.0', sequence '2' on channel 'mychannel' approval status by org:
Org1MSP: false (mismatch: [EndorsementInfo, ValidationInfo, Collections])
Org2MSP: false (mismatch: [ChaincodeParameters])
```

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect --output json
{
        "approvals": {
                "Org1MSP": false,
                "Org2MSP": false
        },
        "mismatches": {
                "Org1MSP": {
                        "items": [
                                "EndorsementInfo (Check the Version, InitRequired, EndorsementPlugin)",
                                "ValidationInfo (Check the ValidationParameter, ValidationPlugin)",
                                "Collections (Check the Collections)"
                        ]
                },
                "Org2MSP": {
                        "items": [
                                "ChaincodeParameters (Check the Sequence, ChaincodeName)"
                        ]
                }
        }
}
```

#### Related issues

- https://github.com/hyperledger/fabric/issues/4428

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 00:17:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4470" class=".btn">#4470</a>
            </td>
            <td>
                <b>
                    Use the errors.Is to check error type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset uses errors.Is to check error type.

Change-Id: Ieae0eaa2527d05fa67aa31afdda42d150fff0980

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

errors.Is is recommened since Go 1.13 to check error type. The error may be wrapped.

More details: https://github.com/golang/go/wiki/ErrorValueFAQ.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 22:10:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4469" class=".btn">#4469</a>
            </td>
            <td>
                <b>
                    Fix comment prefix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The comment prefix should match method name.

Change-Id: I817951e2c94db1705293709fc49f2fc67cf71373

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Fix comment prefix that is not matched with the method name.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-05 21:15:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4467" class=".btn">#4467</a>
            </td>
            <td>
                <b>
                    Remove usage of fmt.Errorf
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset uses the errors pkg to follow the guideline at

https://hyperledger-fabric.readthedocs.io/en/latest/error-handling.html

Change-Id: I36eaac1b429c69195e4af1bb5bb25fc1a2578168

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Remove the usage of fmt.Errorf. Follow the official guideline to change
to the errors package.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 21:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4466" class=".btn">#4466</a>
            </td>
            <td>
                <b>
                    Update add_orderer.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Documentation update

#### Description

Update add_orderer.md to reflect the correct way to add a new orderer to an existing channel.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-04 13:21:35 +0000 UTC
    </div>
</div>

