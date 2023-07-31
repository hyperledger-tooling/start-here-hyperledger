---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/222" class=".btn">#222</a>
            </td>
            <td>
                <b>
                    Upgrade rest package afj to 0.4.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolves #215 

Also switches the rest package to use `indy-vdr`, `askar` and `anoncreds` package set removeing `indy-sdk`

So this is a fairly opinionated upgrade with a fair number of breaking changes against the original rest API. The majority of the potentially controversial changes are to the `SchemaController` and the `CredentialDefinitionController` components as the error handling methodology in the `anoncreds` module is very different to that in `indy-sdk`. There are also some pretty substantial changes to the `ProofController`.

I'm now at the point though where I could use an experienced set of eyes to determine if what I've done is sensible. This isn't quite ready but I feel it's close. Any help/advice from existing maintainers would be greatly appreciated. 

A few todo items still remain to be resolved notably:

- [ ] review configuration and defaults. Some defaults no longer seem to be valid and some configuration items may have been missed. 
- [ ] out-of-band proof API seems to have been completely removed from the framework. My guess looking at the PRs there is that it's somehow been roled into the `oob` functionality but it's unclear how to replicate this or if it's even possible
- [x] on the proof request restrictions there are properties that use a pattern matched key such as `attr::${string}::value` that I cannot reproduce using TSOA. I'm not sure how or if these should be represented.
- [ ] test coverage needs improvement in a few areas and I'd like to do that as part of this PR to make sure I have messed anything up. One place I've noticed and marked is in the credential definition creation tests

Next, whilst the tests are currently passing 2 suites fail due to a cleanup issue that still needs to be resolved. Essentially when two of the tests suites shut down I'm getting an error I'm struggling to debug around the Askar wallet being closed:

```
 WalletError: Error closing wallet': Invalid resource handle

      112 |
      113 |   afterAll(async () => {
    > 114 |     await aliceAgent.shutdown()
          |     ^
      115 |     await aliceAgent.wallet.delete()
      116 |     await bobAgent.shutdown()
      117 |     await bobAgent.wallet.delete()

      at AskarWallet.close (node_modules/@aries-framework/askar/src/wallet/AskarWallet.ts:410:13)
      at WalletApi.close (node_modules/@aries-framework/core/src/wallet/WalletApi.ts:97:5)
      at Agent.shutdown (node_modules/@aries-framework/core/src/agent/Agent.ts:217:7)
      at Object.<anonymous> (tests/webhook.test.ts:114:5)
```

Honestly the entire time I've worked on this the tests have felt a bit fragile, partly because of concurrent testing causing collisions in open wallets. I've done my best to fix some of these issues, but the above failure seems intermittent so I'm not convinced I was entirely successful.

FInally I should point out that up to now I've been relying almost exclusively on the tests here to determine if things are working. I don't know if there's any other things I should be checking, but if there is some guidance would be very helpful.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 13:31:00 +0000 UTC
    </div>
</div>

