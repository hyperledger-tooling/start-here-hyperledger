---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2318" class=".btn">#2318</a>
            </td>
            <td>
                <b>
                    [fix] #2128: Fix `MerkleTree` construction and iteration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

#### when
```rust
    #[test]
    fn leaves_5() {
        let tree = (1..=5)
            .map(|i| Hash::prehashed([i; Hash::LENGTH]).typed())
            .collect::<MerkleTree<()>>();

        for node in tree.iter() {
            dbg!(node);
        }
    }
```

#### before
```
              #0: iteration order
              c7: first 2 hex of hash
        ______/\______
      #8              #1
      f6              c0
    __/\__          __/\__
  #a      #9      #5      #2
  05      00      fc      17
                  /\      /\
                #7  #6  #4  #3
                01  02  03  04
```

#### after
```
              #0: iteration order
              e4: first 2 hex of hash
        ______/\______
      #1              #2
      c0              c1
    __/\__          __/\__
  #3      #4      #5      #6
  fc      17      f6      89
  /\      /\      /\      /\
#7  #8  #9  #a  #b  #c  #d  #e
01  02  03  04  05  00  00  00
```

### Issue
- Closes #2128

### Benefits
- Fixes `MerkleTree::get_leaf`
- Fixes internal alignment and ordering of `MerkleTree`

### Possible Drawbacks
Because of filling the base layer with empty nodes:
- Changes the root hash
- Increases computational cost
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 06:46:37 +0000 UTC
    </div>
</div>

