---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/614" class=".btn">#614</a>
            </td>
            <td>
                <b>
                    Add bytes buffer functions for encoding and decoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
contract c {
	function f() public returns (bytes) {
		bytes data = new bytes(10);
		data.writeUint32LE(102, 0);
		data.writeUint64LE(0xdeadcafe, 4);
		return data;	
	}
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 15:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    Builtin cleanups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-27 12:22:18 +0000 UTC
    </div>
</div>

