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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2942" class=".btn">#2942</a>
            </td>
            <td>
                <b>
                    Unit test flake when rpc server stream not closed (backport #2935)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 21:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2940" class=".btn">#2940</a>
            </td>
            <td>
                <b>
                    Unit test flake when rpc server stream not closed (backport #2935)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2935 done by [Mergify](https://mergify.io).


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
        Created At 2021-09-21 21:46:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2939" class=".btn">#2939</a>
            </td>
            <td>
                <b>
                    Fixed Found Typos
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

- Fixed found typos throughout fabric code

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->


<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
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
        Created At 2021-09-21 16:24:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2936" class=".btn">#2936</a>
            </td>
            <td>
                <b>
                    FAB-2931: do not create a chain if it's already created (backport #2934)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2934 done by [Mergify](https://mergify.io).

Addresses #2931 

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
        Created At 2021-09-20 19:19:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2935" class=".btn">#2935</a>
            </td>
            <td>
                <b>
                    Unit test flake when rpc server stream not closed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

#### Description
This Unit test fails randomly in more recent PR builds(https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40922&view=logs&j=e306c17a-d139-54bf-a475-f5a11259cee7&t=1e3023a5-584f-52f3-49bc-66bd27d27b6d, https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40557&view=logs&j=6b58850f-3858-5a05-33e2-5e41cbf03c4e&t=bddec1cf-ba37-5883-9c3e-fd1e8608f9a1, https://dev.azure.com/Hyperledger/Fabric/_build/results?buildId=40922&view=logs&j=e306c17a-d139-54bf-a475-f5a11259cee7&t=1e3023a5-584f-52f3-49bc-66bd27d27b6d)

Testcase: 
orderer/common/cluster_test.TestSendSubmitWithReport

Analysis/Observation: 
Problem 1: Testcase expects to fail at SubmitRequest after node server restarts with error EOF, but if restart not closed the streams before sendSubmit submitted; test fails. It is random failure. This PR introduces a delay between restart and submitRequest.

Problem 2: Calling t.FailNow() from other than main test go-routine, won't terminate all other subroutines. (which is called in this testcase from require.EqualError(t, err, io.EOF.Error())) This is the reason for the testcase hangs/blocked. https://pkg.go.dev/testing#B.FailNow.  Updated the testcase to signal & terminate the testcase from test main go-routine.

#### Related issues
#2835 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 12:57:55 +0000 UTC
    </div>
</div>

