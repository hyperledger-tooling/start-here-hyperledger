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
                PR <a href="https://github.com/hyperledger/fabric/pull/4523" class=".btn">#4523</a>
            </td>
            <td>
                <b>
                    Make clear of osnadmin remove usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: Id90cea1c9152f2f6c2d0225488eb6e08a5808a68

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset explains more details about `osnadmin remove`.


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
        Created At 2023-11-02 18:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4522" class=".btn">#4522</a>
            </td>
            <td>
                <b>
                    Fix doc link for chaincode access control
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix doc link for chaincode access control.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 17:12:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4521" class=".btn">#4521</a>
            </td>
            <td>
                <b>
                    Directly return the result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: Ic086d2fa7d430c6fa88b92c7b8e99709c3b1569e

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

No need to create the QueryResponseMetadata struct.


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
        Created At 2023-11-02 17:00:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4519" class=".btn">#4519</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc from 1.53.0 to 1.56.3 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump google.golang.org/grpc from 1.53.0 to 1.56.3.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 15:19:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4518" class=".btn">#4518</a>
            </td>
            <td>
                <b>
                    Update doc generation dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update doc generation dependencies to match latest in main branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 19:27:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4517" class=".btn">#4517</a>
            </td>
            <td>
                <b>
                    Verify transactions are well formed when computing the block's data hash instead of externally
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To make sure the function VerifyTransactionsAreWellFormed is called in the right places,
I moved its invocation to the computation of the Fabric's block data hash.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-01 10:46:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4515" class=".btn">#4515</a>
            </td>
            <td>
                <b>
                    Simplify code logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I7b14ef1c54b0d3cb7d5afc4cf21d5e0e6bd36586

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset uses direct error check and allows run code when the criteria is met, which will simplify the code logic.

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
        Created At 2023-11-01 04:00:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4514" class=".btn">#4514</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker to v24.0.7+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also requires updating the following to address compile issues:
- github.com/fsouza/go-dockerclient to v1.10.0.
- github.com/klauspost/compress to v1.13.6.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 16:09:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4512" class=".btn">#4512</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.14
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.2.14.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 15:30:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4511" class=".btn">#4511</a>
            </td>
            <td>
                <b>
                    Release commit for v2.5.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add docs and release notes for v2.5.5 release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 15:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4510" class=".btn">#4510</a>
            </td>
            <td>
                <b>
                    bug fix 4509. Configuration parameters CA and address in peer.deliver…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

Fabric reads the values stored in core.yaml in the peer.deliveryclient.addressOverrides section, but when connecting to orderers through the connect method in the blocksprovider.go file (internal/pkg/peer/blocksprovider/blocksprovider.go) it is using the RandomEndpoint function (endpoint, err := d.Orderers.RandomEndpoint()) located in the connection.go file (internal/pkg/peer/orderers/connection.go) to set up the endpoint that will make the connection. However the RandomEndpoint function does not use the peer.deliveryclient.addressOverrides information read by Fabric.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

https://github.com/hyperledger/fabric/issues/4509

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
        Created At 2023-10-31 12:07:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4508" class=".btn">#4508</a>
            </td>
            <td>
                <b>
                    Switching to use buildx to build docker images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit enables to use `docker buildx` and make use of remote cache while building new images to reuse unchanged layers instead of building them each time, thus speeding up building new Fabric container images.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-31 11:30:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4507" class=".btn">#4507</a>
            </td>
            <td>
                <b>
                    Add error handle for stream
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I8928e64ce09d6f6a0f2f411473d645c46a1b0db5

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset checks the potential returned error from the stream between peer and external chaincode.

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
        Created At 2023-10-30 18:13:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4505" class=".btn">#4505</a>
            </td>
            <td>
                <b>
                    Skip checking well formed-ness for config blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the block is a config block, no point in checking its well formed-ness as it only can contain a single transaction.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-29 21:36:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4504" class=".btn">#4504</a>
            </td>
            <td>
                <b>
                    Verify transactions in a block are well formed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Verify that transactions in blocks appear exactly as their marshaled form after unmarshaling.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-29 21:30:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4503" class=".btn">#4503</a>
            </td>
            <td>
                <b>
                    Verify transactions in a block are well formed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Verify that transactions in blocks appear exactly as their marshaled form after unmarshaling.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-29 21:27:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4502" class=".btn">#4502</a>
            </td>
            <td>
                <b>
                    chore(ci): move to dedicated Fabric runners (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Utilize faster runners for verify CI jobs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-27 15:26:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4501" class=".btn">#4501</a>
            </td>
            <td>
                <b>
                    chore(ci): move to dedicated Fabric runners (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Utilize faster runners for verify CI jobs.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-27 15:25:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4498" class=".btn">#4498</a>
            </td>
            <td>
                <b>
                    fix minor typos for docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix minor typos for docs and comments
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-27 09:35:36 +0000 UTC
    </div>
</div>

