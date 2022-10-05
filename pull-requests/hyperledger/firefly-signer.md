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
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Add filesystem listener interface to KeystoreV3 signer, and move to `pkg`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Moves `internal/filewallet` to `pkg/fswallet`
- Makes it a pure code interface where the use of config YAML is optional
- Changes this directory based wallet to have an in-memory map of addresses
- Adds file listener to detect addition of new key files on disk, and update the in-memory list
- Adds `filenames.primaryMatchRegex` option to extract addresses from any position in filenames
- Removes `filenames.with0xPrefix` option as no longer necessary - the code seamlessly handles either now
- Adds listener code interface, to allow external code to perform per-key processing
   - Called for all keys whether there at `Initialize` time, or added later
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-04 21:16:42 +0000 UTC
    </div>
</div>

