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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3677" class=".btn">#3677</a>
            </td>
            <td>
                <b>
                    enhance:add benchmark test case for txmgmt
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

- Test update

#### Description

add bench mark test for txmgmt, in case for performance enhancement usage.
```
cd ${fabric}/core/ledger/kvledger/txmgmt/
go test -cpuprofile cpu.prof -memprofile mem.prof -bench . --count=5
pprof -http=":8091" ./cpu.prof
```
access http://localhost:8091/ui/ and http://localhost:8091/ui/flamegraph to see flame graph.

<img width="1440" alt="image" src="https://user-images.githubusercontent.com/7820992/194869127-293080b8-31a6-47f2-846f-cd703db95226.png">

<img width="1709" alt="image" src="https://user-images.githubusercontent.com/7820992/194869193-e5429b3c-d010-451a-aa61-f2f22d46beb3.png">


#### Additional details
n/A
<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues
n/A
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

Signed-off-by: Sam Yuan <yy19902439@126.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 06:52:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3676" class=".btn">#3676</a>
            </td>
            <td>
                <b>
                    use matrix to avoid copy my self in github action(pipeline as) code (backport #3617)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3617 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 03:28:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3675" class=".btn">#3675</a>
            </td>
            <td>
                <b>
                    use matrix to avoid copy my self in github action(pipeline as) code (backport #3617)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3617 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 03:27:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3674" class=".btn">#3674</a>
            </td>
            <td>
                <b>
                    use matrix to avoid copy my self in github action(pipeline as) code (backport #3617)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3617 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 03:27:27 +0000 UTC
    </div>
</div>

