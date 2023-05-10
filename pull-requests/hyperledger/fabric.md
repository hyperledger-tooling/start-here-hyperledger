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

As described in issue #4203 .

#### Related issues

Issue: #4203 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 11:58:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4208" class=".btn">#4208</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove ORDERER_TRANSACTION
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I97bdd9fbc60195bbaf7c4486e43dbf7f28bbff66

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

The ORDERER_TRANSACTION type is no longer used, reject it everywhere

#### Related issues

Issue: #3515 #4204
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-07 16:44:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4207" class=".btn">#4207</a>
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-07 15:14:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4201" class=".btn">#4201</a>
            </td>
            <td>
                <b>
                    Restrict WAL usage to node.go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/fabric/issues/4199
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-06 23:30:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4196" class=".btn">#4196</a>
            </td>
            <td>
                <b>
                    system channel clean up - msgprocessor package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Cleaned dependencies on system channel from the msgprocessor package.
2. Removed templator usages.

#### Type of change

- Improvement (improvement to code, performance, etc)
- Test update

#### Description

As described in issue #4189.

#### Additional details

#### Related issues

Issue: #4189.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 14:24:05 +0000 UTC
    </div>
</div>

