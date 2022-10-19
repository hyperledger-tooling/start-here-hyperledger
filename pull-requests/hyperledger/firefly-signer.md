---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Evaluate all FS events: SMB CIFS filesystems mounted do not notify `CREATE`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a Linux environment with a Samba mounted CIFS filesystem, we only seem to get a notification as follows:

```
[2022-10-18T20:52:51.713Z] TRACE FSEvent [WRITE]: /.../keystore/UTC--2022-10-18T20-52-51.648Z-07686308b652040e74189f7a63a0031e6391e234 fswallet=/.../keystore
```

Currently the code only evaluates `CREATE` events, so we need to take the small overhead of the extra `stat()` and filename matching of also handling `WRITE` events.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 20:58:11 +0000 UTC
    </div>
</div>

