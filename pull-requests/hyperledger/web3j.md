---
layout: default
title: web3j
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/web3j
---

# web3j <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/web3j){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2086" class=".btn">#2086</a>
            </td>
            <td>
                <b>
                    Fixing URLs and branches
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
### What does this PR do?
fix for new URL (web3j to hyperledger) including one branch fix (master to main)

### Where should the reviewer start?
doesn't matter, changes are indenpendent for each class / file

### Why is it needed?
branch name and repository owner changed

## Checklist

- [ ] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [ ] I've added a changelog entry if necessary.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-30 12:24:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2084" class=".btn">#2084</a>
            </td>
            <td>
                <b>
                    Bug fix for FastRawTransactionManager.resetNonce
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
Make `FastRawTransactionManager.resetNonce()` reset the nonce

### Where should the reviewer start?
#2002

### Why is it needed?
#### AS-IS
```java
    public synchronized void resetNonce() throws IOException {
        nonce = super.getNonce();
    }
```
#### TO-BE
```java
    public synchronized void resetNonce() throws IOException {
        nonce = BigInteger.valueOf(-1);
    }
```

While the **AS-IS** reset nonce with the current nonce, if `getNonce()` is called, it will return `currentNonce + 1`.

```java
    @Override
    protected synchronized BigInteger getNonce() throws IOException {
        if (nonce.signum() == -1) {
            // obtain lock
            nonce = super.getNonce();
        } else {
            nonce = nonce.add(BigInteger.ONE); // this line will be called
        }
        return nonce;
    }
```

## Checklist

- [x] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [x] I've added a changelog entry if necessary.

fix #2002
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 00:44:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/web3j/pull/2083" class=".btn">#2083</a>
            </td>
            <td>
                <b>
                    Bug fix for BytesType.bytes32PaddedLength
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What does this PR do?
Bug fix for BytesType.bytes32PaddedLength

### Where should the reviewer start?
#2080 

### Why is it needed?
`BytesType.bytes32PaddedLength()` returns incorrect value for lengths greater than 32 and multiples of 32.

[BytesType::bytes32PaddedLength‎](https://github.com/hyperledger/web3j/blob/main/abi/src/main/java/org/web3j/abi/datatypes/BytesType.java#L29)
```java
    @Override
    public int bytes32PaddedLength() {
        return value.length <= 32
                ? MAX_BYTE_LENGTH
                : (value.length / MAX_BYTE_LENGTH + 1) * MAX_BYTE_LENGTH;
    }
```
In case of the `value.length` is 64, 96, 128, ...
It should return 64, 96, 128, ...
However, the results are 96, 128, 160, ...

The corrected code is as follows:
```java
    @Override
    public int bytes32PaddedLength() {
        if (value.length < MAX_BYTE_LENGTH) {
            return MAX_BYTE_LENGTH;
        } else if (value.length % MAX_BYTE_LENGTH == 0) {
            return value.length;
        } else {
            return (value.length / MAX_BYTE_LENGTH + 1) * MAX_BYTE_LENGTH;
        }
    }
```

## Checklist

- [x] I've read the contribution guidelines.
- [ ] I've added tests (if applicable).
- [ ] I've added a changelog entry if necessary.

fix #2080 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 00:18:24 +0000 UTC
    </div>
</div>

