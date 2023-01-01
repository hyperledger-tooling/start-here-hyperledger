---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/481" class=".btn">#481</a>
            </td>
            <td>
                <b>
                    test: use `T.TempDir` to create temporary test directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A testing cleanup. 

This pull request replaces `ioutil.TempDir` with `t.TempDir`. We can use the `T.TempDir` function from the `testing` package to create temporary directory. The directory created by `T.TempDir` is automatically removed when the test and all its subtests complete. 

This saves us at least 2 lines (error check, and cleanup) on every instance, or in some cases adds cleanup that we forgot.

Reference: https://pkg.go.dev/testing#T.TempDir

```go
func TestFoo(t *testing.T) {
	// before
	tmpDir, err := ioutil.TempDir("", "")
	require.NoError(t, err)
	defer os.RemoveAll(tmpDir)

	// now
	tmpDir := t.TempDir()
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-31 09:21:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    Fixing merkle typo - documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: May Rosenbaum <mayro1595@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-28 14:02:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    Remove stale docs folder from main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The docs folder should only exist in the `documentation` branch.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-27 11:01:45 +0000 UTC
    </div>
</div>

