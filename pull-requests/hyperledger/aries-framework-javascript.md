---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1035" class=".btn">#1035</a>
            </td>
            <td>
                <b>
                    feat(bbs): extract bbs logic into separate module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes #948 

Extract the bbs logic into a separate `@aries-framework/module-bbs`. I had to export a lot of the vc stuff from the core bloating the core imports a bit. I think this will be solved when we extract the vc logic into it's own vc package.

For now I've disabled the bbs tests to run on node 17 and 18, so we will have passing CI again, with the knowledge that BBS is broken in node 17 and 18. I also set the package to private for now so that it won't be released with the 0.3.0 release and we have more time to fix it and get it ready for release.

What do we think of the name `@aries-framework/module-bbs`? Should we call it `@aries-framework/bbs-signatures`? It's private for now, so we have room to rename it until we remote the private: true from the package.json

There's is only really ugly hack (one of the first files in the file overview) that has to do with tsyringe injection not allowing nothing to be registered for a token. We have a signing provider that is only used for bbs, and in if you don't register the bbs module it will fail. I didn't want to spend too much time to rework it, so implemented a quick workaround for now


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 10:12:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1034" class=".btn">#1034</a>
            </td>
            <td>
                <b>
                    refactor(proofs)!: createRequest for connectionless proof request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Similar approach as #772, to be able to create a legacy Out-of-Band invitation containing a Request Proof message.

Resolves #997 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 22:46:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1030" class=".btn">#1030</a>
            </td>
            <td>
                <b>
                    Merge branch 'main' into 0.3.0-pre
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merging 0.2.3 and 0.2.4 features into 0.3.x branch:

- All tests pass
- Demo works
- Action Menu module was added to the core for the moment

Hope to not have missed anything. Please double check!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 20:11:49 +0000 UTC
    </div>
</div>

