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
                PR <a href="https://github.com/hyperledger/fabric/pull/2756" class=".btn">#2756</a>
            </td>
            <td>
                <b>
                    Update test network tutorial for new profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

Update create channel tutorial to reflect cleaned up application channel profile in test network configtx.yaml

#### Type of change

- Documentation update


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 21:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2755" class=".btn">#2755</a>
            </td>
            <td>
                <b>
                    added fix to a possible error on many systems
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Error: error parsing transient string: invalid character '\n' in string literal - proposal response: <nil>
Fixed it for all systems

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

<!--- Describe your changes in detail, including motivation. -->
Reached ```Error: error parsing transient string: invalid character '\n' in string literal - proposal response: <nil>``` on running command a base64 command from the tutorial. 
Turns out base64 commands on linux add a newline character to wrap after every 76 characters.

Fixed it by modifying command so that it removes any existing newline characters.

Could have done ```-w 0```, but it is not available in Alpine. 

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
        Created At 2021-07-14 19:57:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2754" class=".btn">#2754</a>
            </td>
            <td>
                <b>
                    [FAB-11334] Scrubs partially constructed/deleted ledgers at peer init
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Peer init will now remove any ledger with status `UNDER_CONSTRUCTION` or `UNDER_DELETION` 
at startup. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Unjoining a peer from a channel will mark the ledger with status UNDER_DELETION
and proceed with the ledger removal.  If the unjoin operation fails, the ledger
will include residue from the partial deletion, leaving the kvledger in a
questionable state.  This commit forces the peer initialization to scan for any
ledgers with an UNDER_DELETION status, removing partial ledgers from the peer 
at startup.

#### Additional details

#### Related issues

- FAB-16035
- FAB-4481
- FAB-17787
- FAB-17801


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 18:49:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2752" class=".btn">#2752</a>
            </td>
            <td>
                <b>
                    FAB-18482 Unable to specify peer's chaincode.externalBuilders as an env variable (backport #2643)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2643 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-13 18:12:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2751" class=".btn">#2751</a>
            </td>
            <td>
                <b>
                    FAB-18482 Unable to specify peer's chaincode.externalBuilders as an env variable (backport #2643)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2643 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-13 18:12:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2750" class=".btn">#2750</a>
            </td>
            <td>
                <b>
                    Ouput Directory For Divergent Results
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

- Several changes were made to the ledger utility tool in preparation for future updates, most notably: output files are now created in a new directory, compare tool no longer overwrites existing files and will throw an error instead, and improved usability and consistency for the outputDir flag
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 21:48:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2749" class=".btn">#2749</a>
            </td>
            <td>
                <b>
                    Fixed a typo in private_data_tutorial
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

- Documentation update

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
        Created At 2021-07-12 13:35:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2748" class=".btn">#2748</a>
            </td>
            <td>
                <b>
                    Replicate block metadata with block while OSN catching up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

While OSN catches up replicating block from the up-to-date replica the consenters' metadata information omitted, i.e.

```
c.support.WriteBlock(block, nil)
```

where `nil` substitutes for block's metadata.

In this commit, the consenters' metadata extracted from the replicated block and being written with the block.

Signed-off-by: Artem Barger <artem@bargr.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-10 23:58:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2747" class=".btn">#2747</a>
            </td>
            <td>
                <b>
                    fixed peer sample config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

peer sample config file description fixed 

- Documentation update

#### Description

peer sample config file description fixed 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-10 08:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2746" class=".btn">#2746</a>
            </td>
            <td>
                <b>
                    Renamed Ledger Binary To Ledgerutil
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
- Renamed the recently merged ledger binary to ledgerutil to avoid confusion with packages that contain actual ledger code 

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->


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
        Created At 2021-07-09 23:09:54 +0000 UTC
    </div>
</div>

