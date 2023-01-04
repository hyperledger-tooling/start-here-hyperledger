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

