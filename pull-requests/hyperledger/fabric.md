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
                PR <a href="https://github.com/hyperledger/fabric/pull/4217" class=".btn">#4217</a>
            </td>
            <td>
                <b>
                    Orderer v3: SmartBFT: eliminate Consnsus.Type in orderer.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: Ieddc902e711de7a0f7dabc76111dde100abb185e

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: SmartBFT: eliminate Consnsus.Type in orderer.yaml

#### Related issues

#4216 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-14 15:29:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4214" class=".btn">#4214</a>
            </td>
            <td>
                <b>
                    Update chaincode_lifecycle.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Content updates - docs #3276
Changing from "new" to "v2.x"

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

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
        Created At 2023-05-10 13:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4213" class=".btn">#4213</a>
            </td>
            <td>
                <b>
                    Update references to system channel in swagger definition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update references to system channel in swagger definition of channel participation API

#### Type of change

- Documentation update

#### Description

As described in issue #4194 .

#### Related issues

issue #4194 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-10 09:07:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4212" class=".btn">#4212</a>
            </td>
            <td>
                <b>
                    test: use `t.Setenv` to set env vars
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

Starting from Go 1.17, we can use `t.Setenv` to set environment variable in test. The environment variable is automatically restored to its original value when the test and all its subtests complete. This ensures that each test does not start with leftover environment variables from previous completed tests.

Reference: https://pkg.go.dev/testing#T.Setenv

```go
func TestFoo(t *testing.T) {
	// before
	os.Setenv(key, "new value")
	defer os.Unsetenv(key)
	
	// after
	t.Setenv(key, "new value")
}
```

#### Additional details


#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 16:02:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4210" class=".btn">#4210</a>
            </td>
            <td>
                <b>
                    system channel cleanup - remove replicator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cleaned dependencies on system channel from the `orderer/common/cluster/replication.go`.

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

As described in issue #4202 .

#### Related issues

Issue: #4202 .
Related PR: #4207 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 13:55:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4209" class=".btn">#4209</a>
            </td>
            <td>
                <b>
                    system channel cleanup - cleanup integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cleaned dependencies on system channel from the integration tests.

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

As described in issue #4203 & #4205

#### Related issues

Issue: #4203 #4205 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 11:58:10 +0000 UTC
    </div>
</div>

