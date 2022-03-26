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
                PR <a href="https://github.com/hyperledger/fabric/pull/3301" class=".btn">#3301</a>
            </td>
            <td>
                <b>
                    new stack image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

<!--- Provide a descriptive summary of your changes in the Title above. -->

Existing software stack image needs updates for both legibility and text.

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)
- Documentation update

#### Description

Just a new graphic image for legibility and updated text.

#### Related issues

https://github.com/hyperledger/fabric/issues/3278


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 21:50:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3299" class=".btn">#3299</a>
            </td>
            <td>
                <b>
                    Add pkgcc.sh script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 11:51:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3298" class=".btn">#3298</a>
            </td>
            <td>
                <b>
                    Retire inactive maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>

#### Type of change

- Documentation update

#### Description

Removing maintainers who are not maintaining.

#### Additional details


#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 23:32:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3297" class=".btn">#3297</a>
            </td>
            <td>
                <b>
                    Bump fastcache
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


- Improvement (improvement to code, performance, etc)


#### Description

- Update fastcache from v1.5.7 to v1.9.0

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues
- #3260

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
        Created At 2022-03-23 17:28:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3296" class=".btn">#3296</a>
            </td>
            <td>
                <b>
                    Add Discord chat to Fabric docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace RocketChat references with Discord in Fabric docs.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 20:56:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3295" class=".btn">#3295</a>
            </td>
            <td>
                <b>
                    fix unittest failure (#3294)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shivdeep Singh <Shivdeep.Singh@ibm.com>

#### Type of change

- Bug fix
- Test update

#### Description

Unittest __snapshot on accumlated bytes condition met__ in `orderer/consensus/etcdraft` was failing due to *Expect* conditions not met. Replaced *Expect* condition with *Eventually* which waits for some time to check for expected condition. 

#### Related issues
- [3294](https://github.com/hyperledger/fabric/issues/3294)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 05:08:02 +0000 UTC
    </div>
</div>

