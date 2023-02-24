---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Release v0.1.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.1.9
                </span>
            </td>
            <td>
                ## What's Changed
* chore: complete release 0.1.8 and prepare 0.1.9 by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3212
* chore: updates to standards doc by @sudeshrshetty in https://github.com/hyperledger/aries-framework-go/pull/3215
* chore: rename operationRequest to operation by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3217
* docs: Storage compatibility matrix by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3214
* docs: Updated storage interface documentation by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3216
* docs: [readme-text] replace digital-hub with encrypted-data-vault by @rolsonquadras in https://github.com/hyperledger/aries-framework-go/pull/3220
* chore: add revocation list 2021 context by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3225
* fix: vc-revocation-list-2021 context by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3226
* feat: In-memory store "ping" method by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3230
* refactor: endpoint as object, goal-code with underscore by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3223
* feat: add HealthCheck for remote kms by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3232
* externalize agent parameters + router by @cnuss in https://github.com/hyperledger/aries-framework-go/pull/3229
* feat: add HealthCheck method to localkms by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3234
* test: Option to skip the "TestProviderOpenStoreSetGetConfig" tests by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3235
* feat: Use new EDV add index endpoint when setting store config by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3237
* refactor: web-redirector with underscore by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3227
* feat: EDV provider - query for multiple tags using AND operators by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3240
* feat: add an option to disable required properties for CredentialParse. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3241
* feat: Add multi-tag support to mem DB by @bstasyszyn in https://github.com/hyperledger/aries-framework-go/pull/3242
* feat: add support of multibase encoding for proofValue. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3244
* refactor: set DIDcomm V1 VS V2 Endpoint support by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3239
* chore: create didcomm v1 and v2 keys in mediator service by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3247
* fix: did doc parsing to properly distinguish V1 vs V2 types by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3250
* chore: add is did comm v2 method to service endpoint by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3251
* feat: Full EDV provider support for AND+OR multiple tag queries by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3252
* chore: add new method to return endpoint type by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3254
* feat: Update EDV provider version for wallet by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3255
* feat: separate cache from token. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3249
* feat: interop support for did service refactor by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3257
* refactor: remote cryptobox URLs renamed to /wrap and /unwrap by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3259
* refactor: re enable remote kms bdd-tests with unwrapKey by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3263
* feat: validate data model of objects saved in a wallet. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3261
* feat: vcwallet support for GNAP authorization by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3266
* refactor: separate didcomm from wallet. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3264
* feat: Legacy Anoncrypt(RFC-0019) DIDComm v1 implementation by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3268
* feat: CL Anoncreds tink primitives by @ashcherbakov in https://github.com/hyperledger/aries-framework-go/pull/3271
* feat: add did document support for alsoKnownAs by @brownoxford in https://github.com/hyperledger/aries-framework-go/pull/3277
* refactor: enable usage of legacy Anoncrypt packer. Make nested forwards while creating forward message. Add legacyForward model by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3272
* chore(deps): bump actions/setup-node from 2.4.0 to 3.4.1 by @dependabot in https://github.com/hyperledger/aries-framework-go/pull/3278
* chore(deps): bump actions/checkout from 2 to 3 by @dependabot in https://github.com/hyperledger/aries-framework-go/pull/3282
* fix: bdd test ci by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3293
* feat: allow custom GNAP header signer in vcwallet command by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3291
* test: interop jwt VCs tests by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3286
* feat: implement did-core JSON-LD `@context` representation by @brownoxford in https://github.com/hyperledger/aries-framework-go/pull/3294
* feat: mediator supports didcomm v1/v2 per-connection by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3303
* feat: add ext db packages to REST Agent (#3269) by @afrancoc2000 in https://github.com/hyperledger/aries-framework-go/pull/3270
* Feat split wallet command by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3276
* feat: Remove warning from secret lock and update documentation by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3307
* fix: move resolve credential manifest from didcommwallet to vcwallet. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3308
* refactor: credential manifest enhancements to match wallet-rendering specs by @HeidiHan0000 in https://github.com/hyperledger/aries-framework-go/pull/3309
* fix: change aries default wallet to didcommwallet. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3313
* test: interop jwt vc ecdsa by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3296
* feat: Add jwt-vc test suites supporting AFGO by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3315
* feat: support of presentation exchange v2. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3312
* fix: small change in schema format for clearness by @HeidiHan0000 in https://github.com/hyperledger/aries-framework-go/pull/3316
* fix: presentation with empty credential fix by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3319
* feat: Connection protocol (RFC-0160) DIDCommV1 implementation by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3295
* feat: allow mediator GetConnections APIs to filter by didcomm version. by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3320
* fix: JWS algorithm for signature suite  by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3322
* fix: vc subject marshal by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3324
* feat: CL Anoncreds Crypto API by @kgoncharov in https://github.com/hyperledger/aries-framework-go/pull/3275
* fix: change validate->Validate by @HeidiHan0000 in https://github.com/hyperledger/aries-framework-go/pull/3328
* feat: implement signer.Alg() by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3332
* test/support ability in AFGO to create and parse vc and vp in JWT format by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3334
* feat: Add client, rest and command handlers for legacy-connection pro… by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3325
* fix: credential manifest omit optional properties by @HeidiHan0000 in https://github.com/hyperledger/aries-framework-go/pull/3336
* feat: CL Anoncreds KMS extension by @kgoncharov in https://github.com/hyperledger/aries-framework-go/pull/3329
* fix: fix afgo interop build by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3341
* feat: KMS storage interface redesign by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3338
* feat: CL Anoncreds Crypto services by @kgoncharov in https://github.com/hyperledger/aries-framework-go/pull/3339
* feat: CL Anoncreds Remote KMS/Crypto by @kgoncharov in https://github.com/hyperledger/aries-framework-go/pull/3343
* refactor: A few refactoring of legacy-connection package by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3342
* feat: wallet.Issue supports jwtvc, verifiable.Credential can hold a jwtvc by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3345
* test: BDD tests for universal wallet JSON-LD support by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3346
* feat: support multi-format VC in presentation exchange by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3347
* feat: Add BDD test for legacy-connection protocol by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3353
* feat: wallet Prove supports creating JWT presentations. by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3350
* feat: Change Credential Fulfillment name to Credential Response by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3360
* feat: BDD tests for legacy connection protocol by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3355
* JSON LD Contexts in JWT VCs by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3357
* test: add JWTVC coverage to wallet VC bdd tests by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3362
* test: jwt format tests in presentation exchange by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3364
* feat: fix format filtering in pEx V2 for JWTVCs, and add bdd tests by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3368
* feat: Validate did configuration for did and domain by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3372
* feat: parse JWT VCs when resolving credential manifests by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3375
* chore: Remove optional "typ" header (JWS) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3378
* chore: Remove adding "iat" when creating JWT Claim by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3380
* feat: Add validation for domain linkage credential in JWT format for did configuration by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3381
* chore: Add interop did configuration test (MS) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3387
* fix: Service type property MUST be a string or a set of strings. by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3389
* chore: upgrade to Go 1.19 by @Abdulbois in https://github.com/hyperledger/aries-framework-go/pull/3382
* fix: don't panic on malformed proof properties by @brownoxford in https://github.com/hyperledger/aries-framework-go/pull/3388
* feat: Add did configuration client by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3391
* Now JWT cred from the presentation is parsed as JWT cred.  Proof not removed. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3399
* fix: jws header by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3401
* fix: id format in vp by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3402
* fix: get DID uri from kid if exists by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3403
* chore: handle PathNested in presexch by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3405
* fix: parse generic ServicePoint by @aholovko in https://github.com/hyperledger/aries-framework-go/pull/3409
* chore: add issuedAt claim to jwt by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3412
* feat: support secp256k1 curve in KMS by @Baha-sk in https://github.com/hyperledger/aries-framework-go/pull/3411
* feat: suppor path_nested in presex. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3416
* chore:  Add auth token provider by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3415
* fix: support of vp referencing in descriptor_map's path. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3417
* feat: Update Tink version, protobuf type by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3413
* feat: Update EDV provider dependency, update golintci, update go docker by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3418
* chore: Controller should be filled in even with relative URL(@base) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3425
* chore: Service priority should be an interface by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3427
* feat: add did core support in resolving service endpoints function by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3429
* feat: sign jwt using a key in an owned DID. by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3433
* feat: command controller for wallet.SignJWT by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3434
* feat: wallet VerifyJWT API to verify compact jwt using DID. by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3435
* refactor: Minimize interfaces required by didsignjwt.SignJWT by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3436
* feat: Add options to VDR Accept by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3439
* feat: refactor didsignjwt to allow decoupling from kms/crypto interfaces by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3437
* fix: didsignjwt Signer interface not exported by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3440
* docs: update standards for both jwt and json-ld vc by @troyronda in https://github.com/hyperledger/aries-framework-go/pull/3442
* chore: add ECDSASecp256k1DER by @fqutishat in https://github.com/hyperledger/aries-framework-go/pull/3444
* chore: DID Config Client is not passing options to DID Config API by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3446
* refactor: Minimize VDResolver interface needed for did config validate by @DRK3 in https://github.com/hyperledger/aries-framework-go/pull/3447
* fix: did service endpoint bug. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3449
* feat: enable ed25519 in jwkkid.BuildJWK() by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3450
* feat: Add SD-JWT Issuer (Flat) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3452
* feat: Add SD-JWT Holder (Flat) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3454
* chore: expose didsignjwt.ResolveSigningVM as a helper API by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3457
* feat: Add SD-JWT Verifier (Flat) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3456
* feat: SD-JWT Holder/Verifier - Process Disclosures by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3460
* feat: Unit test for SD-JWT Flow (Issuer, Holder, Verifier) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3462
* fix: disable JSON-LD validation on JWT credentials by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3465
* feat: Add decoy digests to SD-JWT by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3466
* fix: Presentation Without Holder Binding should end with ~ by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3468
* feat: SD-JWT Issuer: Add Holder Public Key Claim (JWK) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3472
* feat: SD-JWT Holder: Add Holder Binding by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3473
* feat: SD-JWT Verifier: Verify Holder Binding by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3475
* chore: Rename DisclosureSeparator to CombinedFormatSeparator by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3477
* chore: Create SD-JWT without signature by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3480
* feat: Add structured claims option by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3481
* chore: SD-JWT: Support claims with 'vc' verification in issuer by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3483
* fix: Release claims by claim disclosure not by claim name by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3485
* chore: Integration test for structured claim option by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3488
* fix: presex desctiptor format. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3486
* chore: Support verification of 'vc' claims with holder binding by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3490
* feat: SD-JWT: Add NewFromVC to Issuer by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3492
* fix: Move cnf and _sd_alg to vc level by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3495
* feat: verifiable.ParseCredential() supports combined SD-JWT credentials by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3493
* feat: method to marshal SD-JWT VC in combined format for presentation by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3496
* feat: SD-JWT: Add option for non-selectively disclosable claims (issuer) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3498
* feat: method for SD-JWT VC to create non-SDJWT 'display credential' by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3499
* chore: make JWT alg name method exportable by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3501
* fix: allow SD-JWT parsing when sd alg is in cred subject by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3504
* add content type to webhook request by @MajdT51 in https://github.com/hyperledger/aries-framework-go/pull/3159
* Add RemoveCredentialByName to aries js helpers by @borancar in https://github.com/hyperledger/aries-framework-go/pull/3318
* chore: Additional hash algorithms; check for _sd claim by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3503
* feat: Credential.MarshalJSON now marshals all SD-JWT disclosures by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3506
* chore: decode presentation credential in SD JWT format by @mishasizov-SK in https://github.com/hyperledger/aries-framework-go/pull/3507
* feat: ParseCredential recognizes if SD-JWT VC is issuance or presentation by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3510
* feat: creating SD-JWT from VC will leave subject ID as regular field by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3512
* feat: Add support for SD-JWT in presentation exchange by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3509
* chore: Add audience option to issuer by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3513
* fix: prexexch - contains check on filter by @sudeshrshetty in https://github.com/hyperledger/aries-framework-go/pull/3514
* feat: option to pass SD hash alg into Credential.MakeSDJWT() by @Moopli in https://github.com/hyperledger/aries-framework-go/pull/3521
* chore: Add interop test for verifier by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3520
* chore: Additional validation when creating disclosed claims (verifier) by @sandrask in https://github.com/hyperledger/aries-framework-go/pull/3522
* feat: match submission requirements. by @vkubiv in https://github.com/hyperledger/aries-framework-go/pull/3528
* feat: embed claim format designations by @skynet2 in https://github.com/hyperledger/aries-framework-go/pull/3533

## New Contributors
* @cnuss made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3229
* @Abdulbois made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3268
* @ashcherbakov made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3271
* @brownoxford made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3277
* @afrancoc2000 made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3270
* @HeidiHan0000 made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3309
* @mishasizov-SK made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3296
* @kgoncharov made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3275
* @MajdT51 made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3159
* @borancar made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3318
* @skynet2 made their first contribution in https://github.com/hyperledger/aries-framework-go/pull/3533

**Full Changelog**: https://github.com/hyperledger/aries-framework-go/compare/v0.1.8...v0.1.9
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-framework-go/releases/tag/v0.1.9" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-02-22 06:32:11 +0000 UTC
    </span>
</div>

