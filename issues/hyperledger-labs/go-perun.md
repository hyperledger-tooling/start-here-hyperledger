---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/go-perun/issues/179" class=".btn">179</a>
            </td>
            <td>
                <b>
                    ☂️ Beauty fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">good first issue</span><span class="chip">help wanted</span><span class="chip">umbrella</span>
            </td>
            <td>
                List of oddities that we noticed in *go-perun* will be collected here for triage:
- [ ] 1. `channel.Nonce` is modelled as a `*big.Int` but describes a `[]byte` which can cause issues with negative number encoding.
- [ ] 2. `NewFundingReq` returns a `*FundingReq` (per convention) but `Funder.Fund` accepts a `FundingReq`.
- [ ] 3. [eth/Backend.VerifySignature](https://github.com/hyperledger-labs/go-perun/blob/5340aa3f6d9dc59739ad77cd362e0962de435024/backend/ethereum/wallet/backend.go#L69) contains a superfluous `if`
- [x] 4. `wallet.Address` needs only to be an `Encoder`, not `Serializer`. Decoding is handled by the backend anyway. (Done in #194)
- [x] 5. `channel/backend.Verify` gets passed in `Params` but expects the implementation to ignore them (Done in #196).
- [ ] 6. `Params.ID` should be calculated on the fly to avoid inconsistencies. Members of Params are exported, but should be read only (TBD #188).
- [ ] 7. `AdjudicatorReq.Acc` and `AdjudicatorReq.Idx` are not needed for `Adjudicator.Register`. We could create `type RegisterReq` specifically for registering.
- [ ] 9. `Adjudicator.Withdraw` could take the beneficiary as a parameter. (Currently, the beneficiary is a property of the adjudicator.)
- [ ] 10. Add custom errors to the wallet interface: eg. `ErrAccountNotFound` or `ErrWrongAddrType`.
- [ ] 11. Add `NewAssetFundingError` since we also have `NewFundingTimeoutError` and they need each other.
- [ ] 12. Add `NewAdjudicatorReq`.
- [ ] `WithCommitTx` is missing a comment.
- [ ] `local/watcher.go` contains two wrong usages of `Debugf`

Please extend this list.  
:point_right: Related issues will be moved to Milestone *Beautification*.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-06 09:35:43 +0000 UTC
    </div>
</div>

