---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    custom wallets for gateway model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Creating custom wallets is not possible as of now as the store is private property, This will provide an easy way of creating Custom Wallets as each wallet can have its own method of initializing the store and passing it into the wallet, as seen in the filesystem and In-memory wallets. I have used the function in both the default wallets.

```
// WalletFromStore is a simple way that allows to create custom wallets
// based on the user's requirements.
func WalletFromStore(store WalletStore) *Wallet{
	return &Wallet{store}
}
```

Use in filesystem Wallet

```
func NewFileSystemWallet(path string) (*Wallet, error) {
	cleanPath := filepath.Clean(path)
	err := os.MkdirAll(cleanPath, os.ModePerm)

	if err != nil {
		return nil, err
	}

	store := &fileSystemWalletStore{cleanPath}
	return WalletFromStore(store), nil

}
```

similarly also in In-memory wallet.

Following a function similar to [NewCryptoSuite.](https://github.com/hyperledger/fabric-sdk-go/blob/7bf58790be693b74f78e37393781988244b0290b/pkg/core/cryptosuite/bccsp/wrapper/cryptosuiteimpl.go#L17

Wanted to have a simple way like the [Node SDK wallet .](https://github.com/hyperledger/fabric-sdk-node/blob/2b8b63c9d42f3ba96956faae00812afc7c7bb3ad/docs/tutorials/wallet.md)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 08:55:23 +0000 UTC
    </div>
</div>

