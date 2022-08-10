---
layout: default
title: ursa
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/ursa
---

# ursa <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/ursa){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed that there were quite some unnecessary references and small things that could be refactored. If these references and other choices are by-design This PR can be closed and ignored.

It does not alter the functionality one bit except for what seemd to me as an issue in `to_bytes` on the `Sharing` struct.

from:

```rust
    pub fn to_bytes(&self) -> Vec<u8> {
         let mut o = self.identifier.to_be_bytes().to_vec();
         o.append(&mut self.to_bytes()); // This recusively calls itself and should never return?
         o
     }
```

to:

```rust
    pub fn to_bytes(&mut self) -> Vec<u8> {
         let mut o = self.identifier.to_be_bytes().to_vec();
         o.append(&mut self.value);
         o
     }
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 10:02:27 +0000 UTC
    </div>
</div>

