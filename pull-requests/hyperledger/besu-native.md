---
layout: default
title: besu-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-native
---

# besu-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Add gnark mimc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Add gnark mimc to the besu native project

Tested if we have memory link thanks to Visual VM and it's fine

```java
 public static void main(String[] args) {
        for (int j = 0; j < 1000000000; j++) {
            MutableBytes input = MutableBytes.of(new byte[Bytes32.SIZE*16]);
            for (int i = 0; i < 16; i++) {
                input.set(Bytes32.SIZE*(i+1)-i,((byte)((byte) i+(byte) j)));
            }
            byte[] output = new byte[Bytes32.SIZE];
            LibMimc.compute(input.toArrayUnsafe(), input.size(), output);
            System.out.println(Bytes32.wrap(output));
        }

    }
```
![image](https://user-images.githubusercontent.com/26581503/228853172-297b909f-ae97-44b5-aa00-941d7d6358f0.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 13:32:39 +0000 UTC
    </div>
</div>

