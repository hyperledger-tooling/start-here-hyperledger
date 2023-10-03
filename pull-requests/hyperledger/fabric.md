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
                PR <a href="https://github.com/hyperledger/fabric/pull/4455" class=".btn">#4455</a>
            </td>
            <td>
                <b>
                    BFT: orderer deliver headers on cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix
- New feature

#### Description

The orderer delivers blocks with  block.Data=nil when asked for SeekInfo_HEADER_WITH_SIG. However, one needs to avoid mutating the block received from the block iterator, as those are from a cache.

#### Related issues

#4456
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 14:42:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4454" class=".btn">#4454</a>
            </td>
            <td>
                <b>
                    Extend _lifecycle functions on checkcommitreadiness to provide detail of the discrepancies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch updates some _lifecycle functions on checkcommitreadiness to provide details of the discrepancies.

#### Type of change

- New feature

#### Description

I have proposed an extension to lifecycle chaincode checkcommitreadiness to provide details of the discrepancies as shown in  https://github.com/hyperledger/fabric/issues/4428.

As a sub-task stemming from issue #4428, this patch updates some _lifecycle functions on checkcommitreadiness to provide details of the discrepancies.

Once this patch is merged, I will submit the following commit to enhance the command:
- https://github.com/satota2/fabric/commit/9ea8ad11de451139af61cf73281feff656a38d07

#### Additional details

The example of output when executing checkcommitreadiness with inspect flag in the provisional implementation:

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

#### Releated Issues

- https://github.com/hyperledger/fabric/issues/4428


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 08:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4453" class=".btn">#4453</a>
            </td>
            <td>
                <b>
                    Add error check and improve msg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset checks the error when doing yaml marshal, and improves the message when error happens.

Change-Id: I40fb7dbe930bcdc6563078daab50f4f4564c3381

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

* Check the possible error in marshaling;
* Improve message when error happens.

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
        Created At 2023-09-29 17:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4452" class=".btn">#4452</a>
            </td>
            <td>
                <b>
                    Simplify code structure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset simplify the code structure by following Go style.

Change-Id: I47ef0605e17fd4c16a51cd104b8c90d247ce03f7

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

* Use the switch structure;
* Use the error checking directly.

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
        Created At 2023-09-29 16:54:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4451" class=".btn">#4451</a>
            </td>
            <td>
                <b>
                    Update pluggable_endorsement_and_validation.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #2814

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

Node SDK no longer supports chaincode deployment, and therefore the referenced doc page doesn't exist anymore. In this case the entire following sentence should be deleted.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 10:05:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4449" class=".btn">#4449</a>
            </td>
            <td>
                <b>
                    Clean up duplicated check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix duplicated check of file existence and clean up.

Change-Id: If162b6fbfebffd493f345439d346881068916b74

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset removes a duplicated check of the existence of the metadata file, and directly uses the err, which is common following Go style.

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
        Created At 2023-09-26 21:22:13 +0000 UTC
    </div>
</div>

