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
                PR <a href="https://github.com/hyperledger/ursa/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    Adding Aleksandr Petrosyan as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Brent Zundel <brent.zundel@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 16:13:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    fix(wasm): compilable and updated some of the bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Did some local testing and ed25519sha512 and bls seem to work.


```typescript
import { Ed25519Sha512 } from "ursa";
import assert from "assert";

// Test vectors from ursa/libursa/src/signatures/ed25519.rs

const message = new TextEncoder().encode(
  "This is a dummy message for use with tests"
);

const signature = Buffer.from(
  "451b5b8e8725321541954997781de51f4142e4a56bab68d24f6a6b92615de5eefb74134138315859a32c7cf5fe5a488bc545e2e08e5eedfd1fb10188d532d808",
  "hex"
);

const publicKey = Buffer.from(
  "27c96646f2d4632d4fc241f84cbc427fbc3ecaa95becba55088d6c7b81fc5bbf",
  "hex"
);

assert(Ed25519Sha512.verify(message, signature, publicKey));
```

bls has some issues, maybe intentional, with dropping values (see g1 and g2).
```typescript
import assert from "assert";
import { Bls, Generator, SignKey, VerKey } from "ursa";

const msg = new Uint8Array([1, 1, 1]);

const seed = new Uint8Array(32);
const b = new Generator().toBytes();

// Creating of the same two generators as `Bls.sign` drops one and `Bls.verify` as well.
const g1 = Generator.fromBytes(b);
const g2 = Generator.fromBytes(b);

const signKey = SignKey.fromSeed(seed);
const signKey2 = SignKey.fromSeed(seed);

const verKey = new VerKey(g1, signKey);
const signature = Bls.sign(msg, signKey2);

assert(Bls.verify(msg, signature, verKey, g2));
```

Signed-off-by: blu3beri <blu3beri@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 18:08:29 +0000 UTC
    </div>
</div>

