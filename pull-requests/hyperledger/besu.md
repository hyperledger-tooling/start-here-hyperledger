---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6206" class=".btn">#6206</a>
            </td>
            <td>
                <b>
                    Fix log index in transaction receipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Assign log index to transaction receipt according to position in block instead of in transaction.

## Fixed Issue(s)
fixes #6204 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 15:30:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6205" class=".btn">#6205</a>
            </td>
            <td>
                <b>
                    fix collision issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

The idea of this PR is to revert some modification that was made to pass tests  https://github.com/hyperledger/besu/pull/5686.

Therefore, I decided to revert some modification on this PR by fixing the problem differently. Indeed, the idea of the collision test that does not pass is to selfdestruct a contract and recreate it afterwards. Instead of modifying the logic of the accumulator and listing all the storage leaves to be deleted during the selfdestruct, which seems to lead to edge cases, I prefer to let BonsaiWorldstate handle it as before and just load the storage with EMPTY_TRIE_HASH if we detect that it has been cleared before pushing the new slots after recreation. Indeed, the clearing of the storage that is done at the beginning of calculateRootHash removes the storage but does not change the storage root of the contract. Therefore, we falsely believe that the storage is not empty.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 13:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6202" class=".btn">#6202</a>
            </td>
            <td>
                <b>
                    New cli options to limit rewards return by eth_feeHistory 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 06:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6200" class=".btn">#6200</a>
            </td>
            <td>
                <b>
                    Eth peer logging improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span><span class="chip">peering</span>
            </td>
            <td>
                * Moved the full "mismatched network id" message to TRACE and have a brief version at DEBUG
* moved "Disconnect - Outbound" brief message to INFO
* moved the EthPeers {} collection logging to TRACE
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 04:33:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6199" class=".btn">#6199</a>
            </td>
            <td>
                <b>
                    Refactor: improve readability of EthFeeHistory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR does not change anything, just breaks the code into smaller pieces
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 03:54:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6198" class=".btn">#6198</a>
            </td>
            <td>
                <b>
                    Return `address` from the `from` and `to` fields in a GraphQL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Returns an empty `Account` with only the `address` field in the `from` and `to` fields for a 'Transaction` instead of an error in a GraphQL request even if the world state is not retrievable.

In addition an empty `Account` is also returned in the `logger` field.

Sample input:
```
query {
	block (number:10207858) {
		transactions {
			hash
			from { address balance }
			to { address balance }
			logs {
				account { address transactionCount }
			}
		}
	}
}
```

Sample output:
```
{
  "data" : {
    "block" : {
      "transactions" : [ {
        "hash" : "0x8536795a87ab8ba3de721a9b5745f57c3c515221490817737a742d53f3b226d4",
        "from" : {
          "address" : "0xec6a5154ba367f393c565b3597034540ba00c836",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xec6a5154ba367f393c565b3597034540ba00c836",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xeb4da266155ee2c1b92e6e58fe76036e170067ed64084c2d6e4f9349fdb37972",
        "from" : {
          "address" : "0x3f5ce5fbfe3e9af3971dd833d26ba9b5c936f0be",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd4c435f5b09f855c3317c8524cb1f586e42795fa",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xd4c435f5b09f855c3317c8524cb1f586e42795fa",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x1fb9519189c5e0c1fefbd7189e93ce4fb979b5bdf5a7440abcbe903f36cc3f52",
        "from" : {
          "address" : "0x3f5ce5fbfe3e9af3971dd833d26ba9b5c936f0be",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xaec2e87e0a235266d9c5adc9deb4b2e29b54d009",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xaec2e87e0a235266d9c5adc9deb4b2e29b54d009",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x91193212a8c5025e7787999e72a32a382aa3b3d2c8c35bd12370d4381f0edaaf",
        "from" : {
          "address" : "0xa7efae728d2936e78bda97dc267687568dd593f3",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd24cba51e4ba5d56f99b5c59af9f8e1a7f17f719",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x5b7f82af8d88fb040d91fc5c277756d8155e412ace121f7fd46896f31081db32",
        "from" : {
          "address" : "0x0f45c7b7d2c531775509e98d81b0eaf26dbbb8a5",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xdac17f958d2ee523a2206206994597c13d831ec7",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xdac17f958d2ee523a2206206994597c13d831ec7",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x6c48c08efc774b1eb9925d4a337cd11286b82729137a4d27ef99c51e2bfe7e50",
        "from" : {
          "address" : "0x2b5634c42055806a59e9107ed44d43c426e58258",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x9a0242b7a33dacbe40edb927834f96eb39f8fbcb",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x9a0242b7a33dacbe40edb927834f96eb39f8fbcb",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x3c098eddf52a4daa16c86b5a8605f4c9ab54aab25a1503dabc916b1c98a602d2",
        "from" : {
          "address" : "0x2b5634c42055806a59e9107ed44d43c426e58258",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xdf1d6405df92d981a2fb3ce68f6a03bac6c0e41f",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xdf1d6405df92d981a2fb3ce68f6a03bac6c0e41f",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xf9701dd0097859a7a7007e8eb5772aaed907b496811e4dc9a41e8815d9aae194",
        "from" : {
          "address" : "0xd036ec820e931201e5668da8d4a62239a7c79828",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xa22c1b5320108c19db53f58241fd64b105562296",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xa22c1b5320108c19db53f58241fd64b105562296",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xa22c1b5320108c19db53f58241fd64b105562296",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x5fcc269d4e9070c29b042001a12057d5b0f2620b03206fb6994b508f4b3d563c",
        "from" : {
          "address" : "0xc2ba04e89016f417e1219af7ef82a5b6a9214793",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x3506424f91fd33084466f402d5d97f05f8e3b4af",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x3506424f91fd33084466f402d5d97f05f8e3b4af",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x5e6ba1f53a6f249270438401b237cb5c45a8407f28a6f0d02b50bcbe8adc35ea",
        "from" : {
          "address" : "0x8babf0ba311aab914c00e8fda7e8558a8b66de5d",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x68e54af74b22acaccffa04ccaad13be16ed14eac",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x68e54af74b22acaccffa04ccaad13be16ed14eac",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x30742d73cfc1863eceed3f58f50356a0d71736abe4c93873a7888e3427d0d2f6",
        "from" : {
          "address" : "0x00d7e5ee00549efd5e1228d98b32706555f664f7",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x7a9d64336ac7fa9a6b2e68e157608bde80c3b745",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xd3ff33bddd7e192109cc035bbb44304458464f7897dde011f4ced9a59dc7206a",
        "from" : {
          "address" : "0x14b84a0df7e7b09fcca2fe2cfffa4bdb34e797a9",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x9e822665200e10dc38a75f55371bb3c92f716c34",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x58fd21cb5f3704076cd2cb04124924ce9c6a3a26ca43c9b8fdc67a416e6e438b",
        "from" : {
          "address" : "0x1bf8c00d8bfc39d6215afc832926facd86fa1c07",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x452a9f4496e12454fff1f1074a0b4a70a048c4b6",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x280545054a724c6a77e5089eed94941670991f2cd92efbc2b06da14b85f8b19e",
        "from" : {
          "address" : "0xb85a1fb66a67804a017e7b9270db5c6c06c21a3c",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd662cf35bc6c1c91ab3255062934f0fd57680c1b",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x88cd73c3fade14cc0af5f2a75779b0fda16786f123e9411fd3ebfd9933c02698",
        "from" : {
          "address" : "0x599814467c8acbd77b761702f741325af5018a1f",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x34f8e3734918d9bacba97593d34ef942c9682867",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xeacf727508d9fc0f6155aa99d2ca2e4787fd233417153ec912f24106e6a71fd3",
        "from" : {
          "address" : "0x78592fbf9dcef8cf22037024184d8cd86b1682be",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd3fe0cde4d4f8a48ef5dc1c98503dd8aed7ebecc",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x70d85164a2afd717242e5bf758e787d6cf7a937904f8ec67dba31d1fbbf48b84",
        "from" : {
          "address" : "0x91d226108c0432b5e3c3452317e5327668a641bd",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xea2524bb0773de6a5f641aa97294401f116572e7",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xea2524bb0773de6a5f641aa97294401f116572e7",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xcb913488c2544dff9802130f3a9401d5e0fbd150656eaf6ff1b373865ee60e28",
        "from" : {
          "address" : "0xb8001c3ec9aa1985f6c747e25c28324e4a361ec1",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd95fa39d0996ecb5d68ef932ae2bb932c1694836",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6ad4a26aa0f15bcae0d648bec0d0a06aea8742c7e7714980ecfd122bdb51f148",
        "from" : {
          "address" : "0xa08a7c57a076de6cea5dbd6a9d5ed9243b45418d",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x8e46a1c546857679d5e62133fffb9b82d8f72061",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xe6d86a40ea780a7d6f24b60e6a066f45ce4529e5b039ad97b5c5a5187d71c534",
        "from" : {
          "address" : "0x85002559513e9e1e877079007aa760cb827c9447",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x8e46a1c546857679d5e62133fffb9b82d8f72061",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xdbb0ffb7953b42924ae8c7ac3ab13dcee3e1e23bf0d830c5fd87bffcb732e4bb",
        "from" : {
          "address" : "0x6eb2202ffd9080e059b7ca356777771fbc648f1a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xe48c9a989438606a79a7560cfba3d34bafbac38e",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x78025524a8eb2ffa13a54512e9a62f18fb69af93ce9dcf6d5f30325f8d94503f",
        "from" : {
          "address" : "0x27e9f4748a2eb776be193a1f7dec2bb6daafe9cf",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x90d143c36a5ac71111a05cf0d5c0ea90bb936074",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xdc76e954516a04ba88223ef3ce4fd17f28f881f6d69f4e29b57467ded63075b3",
        "from" : {
          "address" : "0x6748f50f686bfbca6fe8ad62b22228b87f31ff2b",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xa0b73e1ff0b80914ab6fe0444e65848c4c34450b",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xa0b73e1ff0b80914ab6fe0444e65848c4c34450b",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x1333d6eb0df61b99bcdfd519bb3522f753675c8042f384d4ada8e04c923fa9e3",
        "from" : {
          "address" : "0x69c4d4c134d1d4750444db54451808f5ee19c743",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xa6a93775f8d316be730ba9d5e99ec466d2ad87b3",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xba619cc51cabf647e07216645c2de435848bbd7597f6f8d645eb104f6c01ac73",
        "from" : {
          "address" : "0xfbb1b73c4f0bda4f67dca266ce6ef42f520fbb98",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xddd460bbd9f79847ea08681563e8a9696867210c",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xddd460bbd9f79847ea08681563e8a9696867210c",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x3486293a808a04bdebda627c4f516ca87f5d6df9978a34ec47cd876c174d10e8",
        "from" : {
          "address" : "0xfbb1b73c4f0bda4f67dca266ce6ef42f520fbb98",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x985dd3d42de1e256d09e1c10f112bccb8015ad41",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x985dd3d42de1e256d09e1c10f112bccb8015ad41",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x3372702ee518534a5e1f016515b66ef6a757b7de32b8ad9dec8354f25fa00b3b",
        "from" : {
          "address" : "0xfbb1b73c4f0bda4f67dca266ce6ef42f520fbb98",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x9f6d6d753ca86e242e5245054bec7b971b3fa483",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xb9ebf58bbf2398f1030abb9599380e4116f633a5b99774bc81ffb60afd376a69",
        "from" : {
          "address" : "0x016bfe5d2f4f14a368ed7222aaacc7934caac694",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x94f82bd45de1ab3ad415889177f71c35f5ed2ccb",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x4fc1580e7f66c58b7c26881cce0aab9c3509afe6e507527f30566fbf8039bcd0",
        "from" : {
          "address" : "0x9c33eacc2f50e39940d3afaf2c7b8246b681a374",
          "balance" : "0x0"
        },
        "to" : null,
        "logs" : [ ]
      }, {
        "hash" : "0xfb6e6c781a4a2253771c570d74f4758912c14c5d59637d072564b60b3f0ff0fe",
        "from" : {
          "address" : "0x9976c40e8186a5e0c2a9d50d55b51f905d10ce52",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x10ab80b78de61a43c55b15a92d077f39d8599c1f",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6bcec1231b72787dea91fb1ac7bcac3570d765f583b1fb878e2dc28b2692b1b8",
        "from" : {
          "address" : "0x5cd9f31e2b1041b2338decf2c4cfeda410c52fee",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x6b175474e89094c44da98b954eedeac495271d0f",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x6b175474e89094c44da98b954eedeac495271d0f",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xae73d5aacff9d4e6962c124dad24d37997f77f09f4fdedf74abcac21b33a6510",
        "from" : {
          "address" : "0x82ec0a9ee5201032c3b2608535d16d682c6261ca",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x11adadd87820a4667fe188168bd3602567496941",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xbd3c3bf1d75c33bd780fb443f50435d1323b8768390116ced717ee4ea24f8101",
        "from" : {
          "address" : "0xf2ad23a749b96f95788a93b820992235c57d5e83",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x25f2e29668c786dafe14bd60a1b132b35b0db5ee",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x0d90cc843b5454046b8ca0d7dc148ac91a2f8087349acc19287bd3e017261680",
        "from" : {
          "address" : "0xa7a7899d944fe658c4b0a1803bab2f490bd3849e",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x2a0c0dbecc7e4d658f48e01e3fa353f44050c208",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x08dc740e8fa7e71d6475e0878033de8d7877083a5820a0257c7f4e280be22bcc",
        "from" : {
          "address" : "0xa7a7899d944fe658c4b0a1803bab2f490bd3849e",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x2a0c0dbecc7e4d658f48e01e3fa353f44050c208",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x0e1d49b5d4dcf39e81c18605fafaead91b0f917a166fe358aea0e0ee2cbeb237",
        "from" : {
          "address" : "0xa7a7899d944fe658c4b0a1803bab2f490bd3849e",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x2a0c0dbecc7e4d658f48e01e3fa353f44050c208",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xd0cbabece55b9803e6b335abcbb5026bc9fd520342b085b72a0d3060a6d00dd7",
        "from" : {
          "address" : "0xa7a7899d944fe658c4b0a1803bab2f490bd3849e",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x2a0c0dbecc7e4d658f48e01e3fa353f44050c208",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x3f2321e021de4e217fcec63bcab339231499a586ab312c16ffbe836073c6aaa6",
        "from" : {
          "address" : "0x9d1b46a7ad520487b00cbf0cd1544c3a6381d4b2",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x2376d2ee1cc40b2e5c777309eca15a1372fbdfcd",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x3145c8037e002a871d96ba1b0623f249a494c60991b5d2b8dae7a0fd9a4e3d78",
        "from" : {
          "address" : "0xb295859980411c257943410ed9b3ba97f9615bdd",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x0b63bbe167df7b6752478d4af07a6235d7631abb",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x801c54a8495ba6b5eb2ec760ca419d1bfea140e96dba07e18bb6dde89c2796b0",
        "from" : {
          "address" : "0xcb40574f1ee9574e4c0b967a218304f844481163",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xccedb68399424e96fd688f1087d1c974db877afe",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xb88e651274313d1a6f630972d1a530f0fbe13e8b4c202a7aeb752d6e6a3f7082",
        "from" : {
          "address" : "0x10133daf5326dd7958bdcbe724c098f48de18138",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xb83f97e471fac857f03064c54d77b96856b79288",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6ab4810233846af9735b7c5c21f233ec0fbaf91e320487d12c04374b3b7ff7ac",
        "from" : {
          "address" : "0xd8aa8f3be2fb0c790d3579dcf68a04701c1e33db",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x29e3b3c76e7ae0d681bf1a6bcee1c0e7d17dbaa9",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x24a718307ce9b2420962fd5043fb876e17430934",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x7e94a8a23687d8c7058ba5625db2ce358bcbd244",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x9308b0bd23794063423f484cd21c59ed38898108",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x049bd8c3adc3fe7d3fc2a44541d955a537c2a484",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xb92ec7d213a28e21b426d79ede3c9bbcf6917c09",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xa8049b0f1c409a58d378e0e41469e824b1bb6e73",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xe23d1142de4e83c08bb048bcab54d50907390828",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xfd8e3f798a8e6f2e52d969420f1bd6d5b6c068e4d7e93e16cdc6acefa97d77bb",
        "from" : {
          "address" : "0xaf8de571c330e2b9b1218ea3e44e1680562e1090",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xadffc29b71fb2dc52dd3491675bd8cd9b23d5638",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x3f9fe25945623f0bce06dcef0166c74cede95decc8e1085a237dd6ebabec3931",
        "from" : {
          "address" : "0xd973c8e4025839f802ccc643fab8175b071b5813",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x170e6863c2ddbd0b86211b5514f5b0491a11fa4d",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xe3c7ad31cb723d0552d7250ea82fc04aeb3497f64a4ca131f7afeeb087f0ba90",
        "from" : {
          "address" : "0x48d641c3d4d9de46f546de37e850290ed6d2141f",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xa18aba501c7b9787210969e769be767deab898ea",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xc452dc136ff45aaa402fbf18b097654722b71a3e323970eb5443b01bdd700651",
        "from" : {
          "address" : "0x92f0c4073aebba17750b5424a17db2eedbff4b03",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd5af805d5429ec16b4059d76854d25a4bb1b7ba9",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xb9c4785d901b5c0dd53becbe20511ced4b36c837ab752ca951566798b8f66057",
        "from" : {
          "address" : "0x11f28505dd776056812e406edba3b68a61cefce2",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd4c435f5b09f855c3317c8524cb1f586e42795fa",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xd4c435f5b09f855c3317c8524cb1f586e42795fa",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x048487ee3860b7b86b77b3d9d0b41e7b1a961086929b9e9a7a42317889429d3c",
        "from" : {
          "address" : "0x4a6aefe670dd494707541b4414cee25b77389489",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x514910771af9ca656af840dff83e8264ecf986ca",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x725483040a2483da1d2784885db3f4d634fa33daec0b8bb39181a888086056e4",
        "from" : {
          "address" : "0xd69dddf3e333aa55298afe7e750f65694206d902",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xe4a7c2160ef5c5e5adafbfab635d0cc39184fd1c",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x0de118904ab984dc329c353eec7aad5cc4c65680ef1e7f1653455855ac93d2b1",
        "from" : {
          "address" : "0xfaa8f14f46a99eb439c50e0c3b835cc21dad51b4",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x0395a255e119bb3c23c89905b600c09e63c84088eb2a48977913d8dab72c5937",
        "from" : {
          "address" : "0xfaa8f14f46a99eb439c50e0c3b835cc21dad51b4",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xdfd4d818ce3b2cccaadf4fd337110ea5b25f49dfaec829b40c5b0c39b7928748",
        "from" : {
          "address" : "0xfaa8f14f46a99eb439c50e0c3b835cc21dad51b4",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x22fd43a10bd0257492c7c1c9930b43755f5acbb8226d10e36d7e06db57be9f8b",
        "from" : {
          "address" : "0xfaa8f14f46a99eb439c50e0c3b835cc21dad51b4",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6b9bccdbd186f03b3974a0e39255a19e8322aadb605ed6e74c20cfe833c251d1",
        "from" : {
          "address" : "0xc6e3e18d0233e496f5e6f0d8168d4cf6319c1bf7",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x0d8775f648430679a709e98d2b0cb6250d2887ef",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x0d8775f648430679a709e98d2b0cb6250d2887ef",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xd30ac93bf425ee2cb09e60a9e66e8786a0015e07ccaa72714c14770c7d8bf3aa",
        "from" : {
          "address" : "0xf535549e464c78b6617616463789ce2f93ffe520",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x73560ddcb0d4396e0d34afbe7de6e3ca81f4c2d8",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x11695744efcdde16078b29e1928e7fbb97f309fcbc8290f11c6b84323649b667",
        "from" : {
          "address" : "0x0031e147a79c45f24319dc02ca860cb6142fcba1",
          "balance" : "0x0"
        },
        "to" : null,
        "logs" : [ ]
      }, {
        "hash" : "0x8b20983d37596028db129148ae370f81b5d4d3cdb762fb904a3604cc3f25d6b7",
        "from" : {
          "address" : "0x44ef0c4cbf10402ece614f2ed0b54bbb4ae52e69",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x797dbfab26308010199f0b18c97c1c554dd119f9",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6d34b99ee77068a012e24a659a1a52c4e935135eac5a6bedf31a315d6069e0a4",
        "from" : {
          "address" : "0xe2877ccafe3cbc813ece98a63aee2b364300d2c1",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x069c97dba948175d10af4b2414969e0b88d44669",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xb62132e35a6c13ee1ee0f84dc5d40bad8d815206",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x069c97dba948175d10af4b2414969e0b88d44669",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x775396e200682be08a924a609da9767d21734bdb1b4fa9404fdc09a0a7decd3e",
        "from" : {
          "address" : "0x9afa066884ce723200438b672c0b8d5769e03a6a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x9992ec3cf6a55b00978cddf2b27bc6882d88d1ec",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x9992ec3cf6a55b00978cddf2b27bc6882d88d1ec",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x332190d3c1d2a9838c53f636793fbf5c84e0a3cf88b9d1f230d66553f2559687",
        "from" : {
          "address" : "0xaefc116514c1d3f590b880e28f3c3a37e440b2ce",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x2b591e99afe9f32eaa6214f7b7629768c40eeb39",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x2b591e99afe9f32eaa6214f7b7629768c40eeb39",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x2b591e99afe9f32eaa6214f7b7629768c40eeb39",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x82ab46fb9dc3a2ff4cd102f249419f14a2d336dc791ba6f2ccee07ed6824e382",
        "from" : {
          "address" : "0xf4fdaba5d04e5575d2b30f9c5eb704b074a146a8",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xc32be7517f37e39c3c17df9ea7397030f06e919f",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x65d8def0e079b8edfd2f54891be8e3d6ea777b45dfaaa42cb7d88741877d8859",
        "from" : {
          "address" : "0x03dcf722ae6231150621c68e9b65992c6a5e6b28",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x7a738effd10bf108b7617ec8e96a0722fa54c547",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x03cbf7948a7a045ea2fc8a1f747028fc0fd87c9ebc54879606406d8c601e06ec",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xe687acda53b49d6fbc6a95ac33713a536dbd6157",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x9a50a79261613fe6793f49cbccce6ecb237ac5359e91138272efad1c647c7ab1",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x085759e1208859df53bfe04230e173fde9b03aed",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6ed52dfcf73488782e18cbec959cc862da39c49fb6accba9e9512f5685b1c1c3",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x69d3c11375a03eaa9e371484756fcd47f7a893df",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xdffb7a6d4548d2ee9e13cdf19d1a361789c4262230f233218ad0c116a6676ba5",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x348c9c1cf6e56a0c02055ac40d24c93bd4404c34",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6f6aa950dfc9339ccfb7820d6322b55a65d20854faa11abd7cecebea62872f48",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x45368456a608fa6501d873f51905f043e38316b2",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x9e06d47fee55881fc08d3d511d65adef143f4f427a2ce9570d899b63b21ff3f7",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x566d42bd4da774a74046c87d255b4f413a1cfd76",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x136649f616bc8a8d70f00880fc9d9c3e708f54daa60103a56f00ea776a39b3c5",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x1134b3084efa9d5d3f60ae701300c57f912070a4",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6c4754dcc6d0d4c5a460aa7518cb0300614d2724c0d94607b4eb1336e067fe2e",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xeb225fdde3f8f6abc832195d5fd696ebb424eec4",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xf1753435f328961532b2b379ffbaf15933deb1d35796a66965299a8c43607a7c",
        "from" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x4e1bd990154789a72d8837d24715c9abe0716211",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x586a7d537f84ff36b464a6656badc1577ec2be0d582db25311babcdd49c357d4",
        "from" : {
          "address" : "0x9e2c5712ab4caf402a98c4bf58c79a0dfe718ad1",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x5f48a3371df0f8077ec741cc2eb31c84a4ce332a",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x23f78c428819c269aa4ef2a8a06ede73d441108d5b672dd9f65240fb298b7942",
        "from" : {
          "address" : "0x98a51196a6155c0176d4d4ba46f34f0fae1c84f5",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xdc97fdaadcbc1c77525b8a1c981865bd2e0425aa",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xdc97fdaadcbc1c77525b8a1c981865bd2e0425aa",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x949c894d1f1a88cd072f46b9a286e62099ccdcccba40291424bdeb0833f07f3e",
        "from" : {
          "address" : "0xfb0fea62f7f211ad3ecf50052760a5331b61883b",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xa22c1b5320108c19db53f58241fd64b105562296",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xa22c1b5320108c19db53f58241fd64b105562296",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xa22c1b5320108c19db53f58241fd64b105562296",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xdd459dd318d6a5e28d8396f679a928b4ec55d4088964c6757151e06a9c51f703",
        "from" : {
          "address" : "0xd24400ae8bfebb18ca49be86258a3c749cf46853",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x44c94b0bf6ac054911e43fcfec33167e3c9bfcf0",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x9b704074ae82855c04c5b127c02ab1c66f6258ab99dba6a778bf5243fd0c3c53",
        "from" : {
          "address" : "0x999d1ce359692aebc26cd969a31d47d150128600",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x142a251c1ccddffecd051f3d903c4eed4c8538ab",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x15ca6d5639429610393e977711743dabebfede3231a184048797b381c57c13e6",
        "from" : {
          "address" : "0x085587bcd6202560c88c70c7afde04edadc1acef",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xd7b9a9b2f665849c4071ad5af77d8c76aa30fb32",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x6c65a26a5a915102f7476558c8aa739109ff3f1c13c40263cc48d147e7b7b06e",
        "from" : {
          "address" : "0xa2f1615ec191f8edaa64cc4da065defa40a964fe",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x1942e46c4b69b9d0768608fc599734884cf8cba8",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xd4b7722b999c430a56b0b1a3cc78cf7ed2484c7c",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x1942e46c4b69b9d0768608fc599734884cf8cba8",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xf63479faef9d4a8aa658470882795d7cb4ee05d7ef01b88eccbccadc75f47535",
        "from" : {
          "address" : "0x5e12c7a25d14bd32c4a88c04fc54d1d420518468",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x3046ccb64ec6c5a42eadfc87add384a09439d3cbea6ef57572ec53963627ac30",
        "from" : {
          "address" : "0xc9ad06d3032191434f75ffabd4245768e0e80578",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x5acc84a3e955bdd76467d3348077d003f00ffb97",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x56b04363a494424055a551d8219b89bb9de68df5354fd5d78988fffb0f81c0f7",
        "from" : {
          "address" : "0x0cc75b6bec8aa14585549ebf2f902d103f6fb7e6",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x85eba557c06c348395fd49e35d860f58a4f7c95a",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x85eba557c06c348395fd49e35d860f58a4f7c95a",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x24df25b13d6c0f3a6c0421b0db8e4c71aac4854c3fec6300e19775fdcc79153f",
        "from" : {
          "address" : "0x7b8003088fe1a333eab1461b1f5a404220ad192a",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xbcf935d206ca32929e1b887a07ed240f0d8ccd22",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xbcf935d206ca32929e1b887a07ed240f0d8ccd22",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0xbcf935d206ca32929e1b887a07ed240f0d8ccd22",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x5f7d7bcc7d16e805a01d8d472b79b1d89cbc8c82a90867cc444d42a66e719d49",
        "from" : {
          "address" : "0x40fa2aa83d2766a37ecb4c22579a7c03266a0ed6",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xdac17f958d2ee523a2206206994597c13d831ec7",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xdac17f958d2ee523a2206206994597c13d831ec7",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x75e3ebf3325d35fda113ecf2933dac6ab67fb210fe643f9d7dccffb61695af0e",
        "from" : {
          "address" : "0x831beaa8f46968b8599500616cff24b6e914f5be",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x6b175474e89094c44da98b954eedeac495271d0f",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x6b175474e89094c44da98b954eedeac495271d0f",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xec3d8deaf2b69f244d732fe8f64d2034bc1bd3ec9e4573ccaae9956e6247b2af",
        "from" : {
          "address" : "0x370ba35ad49e13621c68031f5393e11f0a45058d",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x823135396aeb306f77ecaf38717eb68c6b289ab4",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xc8df311430cf081b981673bbeb9e02d6d1790e9b563ecf2015db660fb02adb95",
        "from" : {
          "address" : "0x4dcb10b8657c22bbcf550deb2d3708546b5ed34b",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x9b7460e9e5b8182da8304e443064cfd6eb7758a5",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x9a61ebcaa09cc7d4c2aea0afd477e947cae56193f0aa7b6b75d24ccc2a07fd3e",
        "from" : {
          "address" : "0xe542915791423c04cda11443a84212370773ecc1",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x8889ec21f75a5990d63ba467a1910608cd3b5d6c",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x0dcb65677d7ec73344b4022e1768ae06a20f95166ee18419e4a3616f5e49753e",
        "from" : {
          "address" : "0x86ef61715eb3da8ca2bb0cf8442c67f30a8e0b5c",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xdfb8bbda2f41cb5677c94a48becac8ef7911a813",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xfa7bfdc313950284ff962ced983f74a2b5969dc9c1184db9de6785008c7ab434",
        "from" : {
          "address" : "0xb59a675bf182ebf75a85a4bd754de8da80813398",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xfce1b716bb074a0809f01bb7d18a65fbf7583e38",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x1d2cd5fde05d4f6c7035bcdffd953d271a1526b7e1de383d83d8fbab4a90809f",
        "from" : {
          "address" : "0x2c45d68a289a8d1088e63bffb9b96f5b88015bf9",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x8527a63a1dbbef963d7479f94c15ec4d0fc3285d",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x63d52a5dafe278860b0486504b57b1d364b37413",
            "transactionCount" : "0x0"
          }
        }, {
          "account" : {
            "address" : "0x8527a63a1dbbef963d7479f94c15ec4d0fc3285d",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xf952cb1d7d8059d3e3d88dfcf0e6a14b6019c02406b789249922124b1cbf7245",
        "from" : {
          "address" : "0xb3a11017ddfb81f60d3ddb24db66f846eb76a4c3",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x512629af096bb392640bf0722f6650e43eb41281",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x34fe42e0a14e402c62ec31a931ab32fb4f096e169f89ce3dac0507326a9e7700",
        "from" : {
          "address" : "0xb0cfce6890c1c4fba2adef42d4ceeb35941525e2",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xac54b0f52f314f1efbef245a5416fd5d7e381b71",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0xbb91b9b9111b010146a84a85da55ee0d2da588ac30a3fee963ddf4e8da7fa8c5",
        "from" : {
          "address" : "0xfcc7fdaf6d0ae5e857935af8af6e740845596ace",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xac54b0f52f314f1efbef245a5416fd5d7e381b71",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x867f637f7e1f3f72edc502039c29aa187c83f1ddc893f96afad77d18475f89e7",
        "from" : {
          "address" : "0xc70b4222340a8f53136ecea573a6ae01105355d7",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xaa7a9ca87d3694b5755f213b5d04094b8d0f0a6f",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0xaa7a9ca87d3694b5755f213b5d04094b8d0f0a6f",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x62ec14a92107c90467a056da03b6029b429e4f88dde1123b5eabf8404ee19a40",
        "from" : {
          "address" : "0x6425bb021dabd5d6b443a1ab47b003a1b7a27d4b",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x61935cbdd02287b511119ddb11aeb42f1593b7ef",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x61935cbdd02287b511119ddb11aeb42f1593b7ef",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x30e9b76c86d52190ee110b20e85b2d936028f44dc93115f220fda29544658c2c",
        "from" : {
          "address" : "0x71f429c0375e7f4031d1e505d2533c1386b29183",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x50701f6d97fd8a0dbda52c677a2891648d6641d6",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x50701f6d97fd8a0dbda52c677a2891648d6641d6",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0xfdb48d94e2bc9679e5cc8135e6d56dcfe5d0a77bb92add6ff651633b6fbc06f6",
        "from" : {
          "address" : "0x71f429c0375e7f4031d1e505d2533c1386b29183",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x50701f6d97fd8a0dbda52c677a2891648d6641d6",
          "balance" : "0x0"
        },
        "logs" : [ {
          "account" : {
            "address" : "0x50701f6d97fd8a0dbda52c677a2891648d6641d6",
            "transactionCount" : "0x0"
          }
        } ]
      }, {
        "hash" : "0x1a9ec86f16448b0ad03c28905e6ce1dfa713160e28d96b9f6547d943ad46af10",
        "from" : {
          "address" : "0x6420b8196918fc12b377d25d889b939c0b98df57",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x057b6b501bd51b3499e2f368c380604f6311513e",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x387aed8dc15a92325e48c4b894ed7ada24f9bba80e334661b82c968f99f45195",
        "from" : {
          "address" : "0xa8fe18d40befb1fff9ff9781dd70ec3682cd37a1",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0x4fed1fc4144c223ae3c1553be203cdfcbd38c581",
          "balance" : "0x0"
        },
        "logs" : [ ]
      }, {
        "hash" : "0x149e53c97ab7bd3758681a5f0b99b2b96e6853a087487eb493313667076c783a",
        "from" : {
          "address" : "0xdc4f7d4cb9565ab4968a1bae9514208dc5907182",
          "balance" : "0x0"
        },
        "to" : {
          "address" : "0xe779e9dc0977e560dde435be0f8a53aa10a6e937",
          "balance" : "0x0"
        },
        "logs" : [ ]
      } ]
    }
  }
}
```

## Fixed Issue(s)
fixes #6182 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 03:36:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6197" class=".btn">#6197</a>
            </td>
            <td>
                <b>
                    [MINOR] update GHA checkout action to v4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/actions/checkout/releases/tag/v4.0.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 02:20:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6195" class=".btn">#6195</a>
            </td>
            <td>
                <b>
                    Refactor: Move rpcGasCap and rpcMaxLogsRange to apiConfiguration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Move rpcGasCap and rpcMaxLogsRange to apiConfiguration
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 23:35:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6194" class=".btn">#6194</a>
            </td>
            <td>
                <b>
                    Fix Docker image name clash between Besu and evmtool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

If Gradle property `dockerArtifactName` is specified, then both Besu and `evmtool` Docker images will use it has name, resulting in one overriding the other. 
The fix in this PR is to always add the `-evmtool` suffix to the `evmtool` Docker image
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 16:56:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6193" class=".btn">#6193</a>
            </td>
            <td>
                <b>
                    verkle trie integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 16:10:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6191" class=".btn">#6191</a>
            </td>
            <td>
                <b>
                    Acceptance test for Clique when configured to not create empty blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 11:33:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6190" class=".btn">#6190</a>
            </td>
            <td>
                <b>
                    Allow a transaction selection plugin to specify custom selection results
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

With this PR a transaction selection plugin can extend TransactionSelectionResult to implement its custom return values.
Plus a couple of log fixes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 17:18:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6189" class=".btn">#6189</a>
            </td>
            <td>
                <b>
                    Update OpenJDK latest Docker image to use Java 21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Switched base image to `ubuntu:rolling`, that follow any stable Ubuntu release, currently 23.10) since OpenJDK Java 21 is not available on latest LTS Ubuntu.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 11:43:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6188" class=".btn">#6188</a>
            </td>
            <td>
                <b>
                    Add experimental x-trie-log subcommand for one-off backlog prune
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Part of https://github.com/hyperledger/besu/issues/5390

## TODO

- [x] Test on a throwaway mainnet node: https://github.com/hyperledger/besu/pull/6188#issuecomment-1820156907
  - took **8m 48s** to prune 293458 trie logs (18 GB) on ~5 week old node
- [ ] Test on one of our oldest nodes to understand duration - my guess is it will be in the order of minutes, hopefully less than 1 hour.
- [ ] If it's really slow, could optimise by loading all trie logs once and reuse for count as well as prune (or just prune instead of count).

## To install on a node

```
cd /opt/besu
sudo wget -O 6188.tar.gz https://output.circle-artifacts.com/output/job/a7a06df9-cf33-4115-89d1-413c86facd71/artifacts/0/distributions/besu-23.10.3-SNAPSHOT.tar.gz
sudo tar zxf 6188.tar.gz --transform s/besu-23.10.3-SNAPSHOT/6188/
time sudo /opt/besu/6188/bin/besu --config-file=/etc/besu/config.toml storage x-trie-log count
```

## Usage and examples

```
$BESU storage x-trie-log -h
Usage: besu storage x-trie-log [-hV] [COMMAND]
Manipulate trie logs
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
Commands:
  count  This command counts all the trie logs
  prune  This command prunes all trie log layers below the retention threshold,
           including orphaned trie logs.
```

```
$BESU --genesis-file=genesis.json --data-path=besu --data-storage-format=BONSAI storage x-trie-log count
...
Counting trie logs...
trieLog count: 512
 - canonical count: 512
 - fork count: 0
 - orphaned count: 0
```

```
$BESU --genesis-file=genesis.json --data-path=besu --data-storage-format=BONSAI storage x-trie-log prune
```

```
$BESU --genesis-file=genesis.json --data-path=besu --data-storage-format=BONSAI --Xbonsai-trie-log-retention-threshold=512 --Xbonsai-trie-log-pruning-limit=513 storage x-trie-log prune
...
Counting trie logs before prune...
trieLog count: 615
 - canonical count: 512
 - fork count: 0
 - orphaned count: 103

Total to prune = 615 (total) - 512 (retention threshold) =
=> 103

Estimated number of batches = max(103 (total to prune) / 513 (batch size), 1) = 1

Pruning batch 1
-----------------
2023-11-20 19:45:19.639+10:00 | main | INFO  | TrieLogPruner | Loading first 513 trie logs from database...
2023-11-20 19:45:19.649+10:00 | main | DEBUG | TrieLogPruner | Pruned 91 orphaned trie logs from database...
2023-11-20 19:45:19.649+10:00 | main | INFO  | TrieLogPruner | Loaded 422 trie logs from database
2023-11-20 19:45:19.657+10:00 | main | DEBUG | TrieLogPruner | pruned 0 trie logs from 0 blocks
Number pruned in batch = 91
Running total number pruned =
=> 91 of 103

Pruning batch 2
-----------------
2023-11-20 19:45:19.657+10:00 | main | INFO  | TrieLogPruner | Loading first 513 trie logs from database...
2023-11-20 19:45:19.665+10:00 | main | DEBUG | TrieLogPruner | Pruned 12 orphaned trie logs from database...
2023-11-20 19:45:19.665+10:00 | main | INFO  | TrieLogPruner | Loaded 501 trie logs from database
2023-11-20 19:45:19.666+10:00 | main | DEBUG | TrieLogPruner | pruned 0 trie logs from 0 blocks
Number pruned in batch = 12
Running total number pruned =
=> 103 of 103

Trie log prune complete!

Counting trie logs after prune...
trieLog count: 512
 - canonical count: 512
 - fork count: 0
 - orphaned count: 0
 ```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 10:22:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6187" class=".btn">#6187</a>
            </td>
            <td>
                <b>
                    consider peer reputation score when deciding to disconnect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">peering</span>
            </td>
            <td>
                Noticed in peering logs we are disconnecting quite useful peers with timeouts and "useless responses". This exacerbates peering issues because we are quite early to disconnect, whereas if we just wait a bit longer the peer can still be useful. More of an issue in low peer count networks. 
* consider peer reputation score when deciding whether to disconnect peer for repeated timeouts/useless responses
* increase threshold for timeout counts
* decrease score points deducted for timeout/useless response


```
➜  besu grep  "Disconnect - Outbound" besu03.log
2023-11-17 17:47:27.730+10:00 | nioEventLoopGroup-3-5 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x0b TIMEOUT - 0x45d5... - 5 peers left
2023-11-17 17:49:10.232+10:00 | nioEventLoopGroup-3-1 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x0b TIMEOUT - 0xcbba... - 4 peers left
2023-11-17 18:02:33.476+10:00 | nioEventLoopGroup-3-8 | DEBUG | EthProtocolManager | Disconnect - Outbound - 0x03 USELESS_PEER - 0x6a7... - 3 peers left
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 05:47:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6186" class=".btn">#6186</a>
            </td>
            <td>
                <b>
                    comment out flaky part of acceptance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">flake</span>
            </td>
            <td>
                this particular test is flaky. There are other tests for the same class that work more reliably. 

Example of flaky fail -
https://app.circleci.com/pipelines/github/hyperledger/besu/25195/workflows/a5a40b6e-0f1d-4ac3-87e6-108bcce92b9e/jobs/164640
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 05:41:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6185" class=".btn">#6185</a>
            </td>
            <td>
                <b>
                    Add Experimental RockDB Subcommand for printing usage per column family
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Pretty much a lift and shift of @ahamlat's https://github.com/ahamlat/RocksdDB-Column-Families-Size

```
➜  besu git:(rocksdb-usage-subcommand) $BESU storage x-rocksdb usage --help
Usage: besu storage x-rocksdb usage [-hV]
Prints disk usage
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
  
➜  besu git:(rocksdb-usage-subcommand) $BESU storage x-rocksdb --help
Usage: besu storage x-rocksdb [-hV] [COMMAND]
Print RocksDB information
  -h, --help      Show this help message and exit.
  -V, --version   Print version information and exit.
Commands:
  usage  Prints disk usage
```

```
$BESU --data-path=/tmp/besu storage x-rocksdb usage
****** Column family 'BLOCKCHAIN' size: 7 KiB ******
Number of keys : 70
Number of live snapshots : 0
Total size of SST Files : 4 KiB
Size of live SST Filess : 4 KiB
Column family size (with getColumnFamilyMetaData) : 4 KiB

****** Column family 'ACCOUNT_INFO_STATE' size: 1 KiB ******
Number of keys : 2
Number of live snapshots : 0
Total size of SST Files : 1 KiB
Size of live SST Filess : 1 KiB
Column family size (with getColumnFamilyMetaData) : 1 KiB

****** Column family 'TRIE_BRANCH_STORAGE' size: 1 KiB ******
Number of keys : 7
Number of live snapshots : 0
Total size of SST Files : 2 KiB
Size of live SST Filess : 2 KiB
Column family size (with getColumnFamilyMetaData) : 2 KiB

****** Column family 'TRIE_LOG_STORAGE' size: 5 KiB ******
Number of keys : 103
Number of live snapshots : 0
Total size of SST Files : 7 KiB
Size of live SST Filess : 7 KiB
Column family size (with getColumnFamilyMetaData) : 7 KiB

****** Column family 'VARIABLES' size: 1 KiB ******
Number of keys : 6
Number of live snapshots : 0
Total size of SST Files : 2 KiB
Size of live SST Filess : 2 KiB
Column family size (with getColumnFamilyMetaData) : 2 KiB
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 02:05:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6183" class=".btn">#6183</a>
            </td>
            <td>
                <b>
                    Revert "fix tests collisions"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit ee7c22ca8b6f591e378b5cec34f2289b1711490e.

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This change from the bonsai reference test worldstate pr #5686 seems to be causing a regression on goerli for block [#9727365](https://goerli.etherscan.io/block/9727365)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-18 07:03:14 +0000 UTC
    </div>
</div>

