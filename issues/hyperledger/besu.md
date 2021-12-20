---
layout: default
title: besu
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2756" class=".btn">2756</a>
            </td>
            <td>
                <b>
                    Add data-path to error message re chain data mismatch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                eg if I start besu with default --data-path and I've already forgotten what the default value is, this will save me looking it up. 

### Description
As a Besu user, I want to see the effective data-path in the error message so that I can delete it if switching between networks. 

### Acceptance Criteria
* Actual/effective data-path is printed out in the error message when genesis block mismatch.

### Steps to Reproduce (Bug)
1. Start besu with --network=rinkeby
2. stop besu
3. start besu with --network=ropsten

**Expected behavior:** [What you expect to happen]
```
Supplied genesis block does not match stored chain data in </path/to/data/path/dir>
Please specify a different data directory with --data-path or specify the original genesis file with --genesis-file.
```
**Actual behavior:** [What actually happens]
```
Supplied genesis block does not match stored chain data.
Please specify a different data directory with --data-path or specify the original genesis file with --genesis-file.
```
**Frequency:** 
every time the genesis block doesn't match

### Additional Information


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 03:03:47 +0000 UTC
    </div>
</div>

