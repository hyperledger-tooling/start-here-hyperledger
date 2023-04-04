---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    test: use `t.TempDir` to create temporary test directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request replaces `ioutil.TempDir` with `t.TempDir`. We can use the `t.TempDir` function from the `testing` package to create temporary directory. The directory created by `t.TempDir` is automatically removed when the test and all its subtests complete. 

Reference: https://pkg.go.dev/testing#T.TempDir

```go
func TestFoo(t *testing.T) {
	// before
	dir, err := ioutil.TempDir("", "")
	assert.NoError(t, err)
	defer os.RemoveAll(dir)

	// now
	dir := t.TempDir()
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 17:38:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    Fixing support for legacy configs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                for https://github.com/hyperledger/firefly/issues/1244

Still need to support the old configurations in which policyengine.simple is provided.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 18:29:00 +0000 UTC
    </div>
</div>

