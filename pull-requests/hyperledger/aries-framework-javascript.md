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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/889" class=".btn">#889</a>
            </td>
            <td>
                <b>
                    fix(oob): allow legacy did sov prefix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Fixes #875 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 09:45:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/888" class=".btn">#888</a>
            </td>
            <td>
                <b>
                    fix: remove usage of const enum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Fixes #884, see the issue for why we can't use const enums
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 08:07:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/887" class=".btn">#887</a>
            </td>
            <td>
                <b>
                    feat(credentials): find didcomm message methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Adds `findProposalMessage`, `findOfferMessage`, `findRequestMessage`, `findCredentialMessage` methods to the credentials module to be able to access the did comm message associated with a credential exchange.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 07:45:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/886" class=".btn">#886</a>
            </td>
            <td>
                <b>
                    feat: delete w3c credential record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a method to the W3cCredentialService to remove a credential record from storage. I also renamed a few properties and methods because their previous names were somewhat misleading.

- feat: add method to remove w3c credential
- refactor: rename methods and props for consistancy

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 18:49:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    fix(connections): allow ; to convert legacy did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Older dids use `;` as an identifier separator instead of the now used `#`. So an id of `did:sov:123;indy` would be normalized to `#did:sov:123;indy`. We now check when converting a legacy did doc to a new did doc whether an `;` character is in place and the `#` isn't and we will handle it correclty so it parses to `#indy`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 15:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/881" class=".btn">#881</a>
            </td>
            <td>
                <b>
                    refactor!: add agent context
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">multitenancy</span>
            </td>
            <td>
                This is a big pull request, but doesn't change any functionality of the agent. All services, repositories etc.. now use agent context so we can start using them as stateless services for multitenancy (as described here: https://hackmd.io/vGLVlxLvQR6jsEEjzNcL8g#Agent-Context).

This doesn't change the public API of the framework, but because of the large number of changes and also the implications for custom modules I've marked this as a breaking change.

Will add more detailed migration docs later on, but generally you have to update your modules to now inject the agent context object and pass that around to services. See the `DummyModule` for an example: https://github.com/TimoGlastra/aries-framework-javascript/blob/317dc779d8ff88921fa6333ed3490ae77784f1ff/samples/extension-module/dummy/DummyModule.ts


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 10:02:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    fix(credentials): miscellaneous typing issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Fixes some issues encountered in the typing. Mainly:
- export the messages types from the core packages
- prepend `V1` and `V2 to all credential interfaces to avoid conflicts in interface names
- use `string` as type for `protocolVersion` instead of `v${string}` to make it work with tsoa
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-19 08:47:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/879" class=".btn">#879</a>
            </td>
            <td>
                <b>
                    chore(release): v0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release version 0.2.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 18:25:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/878" class=".btn">#878</a>
            </td>
            <td>
                <b>
                    ci: fix lerna version detection based on tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes lerna version detection for next release. Lerna will use the latest tag to determine the latest released version. As we create a tag for each commit we need to remove all pre-release tags so we can determine the last stable release. It also excludes the private packages that have been added since 0.1.0 (extension-module and demo) from the release / changelog creation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 17:34:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/877" class=".btn">#877</a>
            </td>
            <td>
                <b>
                    feat(credentials): add get format data method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.2.0</span>
            </td>
            <td>
                Adds a `getFormatData` method to the credentials module to make it easier to retrieve the credential format data for a credential record.


You use it like this:
```ts
const formatData = await agent.credentials.getFormatData(credentialExchangeId)
```

it will return an object with the `proposal`, `offer`, `request`, `credential` keys each containing format keys with their payloads. The return type is fully typed because we define the payloads of the format attachments in the `CredentialFormat` interface (see `IndyCredentialFormat`). It returns the JSON encoded variant of the payloads (like it is send over the wire), not the class instance. This is mainly done because we don't have classes defined for each of the payloads and this also makes it harder to use it over in e.g. the AFJ rest server.

An example of the returned value:

```json
{
      "proposal": {
        "indy": {
          "schema_issuer_did": "GMm4vMw8LLrLJjp81kRRLp",
          "schema_id": "q7ATwTYbQDgiigVijUAej:2:test:1.0",
          "schema_name": "ahoy",
          "schema_version": "1.0",
          "cred_def_id": "GMm4vMw8LLrLJjp81kRRLp:3:CL:12:tag",
          "issuer_did": "GMm4vMw8LLrLJjp81kRRLp"
        }
      },
      "offer": {
        "indy": {
          "schema_id": "TL1EaPFCZ8Si5aUrqScBDt:2:schema-720e72db-658d-49a7-bb0f-df5b8f06e53f:1.0",
          "cred_def_id": "TL1EaPFCZ8Si5aUrqScBDt:3:CL:2490:default",
          "key_correctness_proof": {
            "c": "42066973570095896819081982147997332108675745993570955998740648806660333903631",
            "xz_cap": "570132593605620021757947283571997732612916664583477428247001260768335667066780444787685088673075654835932882503762232731965687100713588497051144906523612431947288176830103389016390392656613247870761944244665321578245050989779999670651087271342900772508286334418303889268489348089568092139003772638206637287240399659749164051691647072774093680555480531158980363280332452938411949698244792496371450057976052631013913219818275311821295801749766504644633059832261790129909513636840901072116491990733259270113325714096498251243522190217107000729836865090452964038956193787247243249117194650376704869822287567855881749627876863161738068815723606161776680320596127905940286143264413119165000552545572",
            "xr_cap": [
              [
                "master_secret",
                "666172621620774367467316536897944483573637632166344176949756030855324387088784971709157308384444962002186379868280288320214433223266643004212485329604715478637425321821867692496910279999700377334391694492600280421215517651691504027681688992813684962438759417089956224665589199380927502204373651581977643333214742182083092434809616523796669423019930292671447880988340279850987452117757598698092946827440961924686573263211642319645687714421679982973749970356778990993071880191005822180967302131139647516540318104055327168161273033986518032511430855888276895228251613687175689215998779699191401294967322597319549575281154060786283181012465341967029256647053547727988600853644820668238691847178524"
              ],
              [
                "profile_picture",
                "487142493300360724982682494894226906918624444006677981179687897024790792243759960230742060972504457511982302639382993600485820666292385718684572089559092995495135774375413598766810582381265948779479248338693873964981401570727348629566325988795020688746668275379768952587951556298412594034060134176324132074978909079815364760668306251983065125721079593647579402916142119763827587237630920808574899029497800283973936720808999906564085304471270564084025904291019319303343380088387466190462897512479963605859476201648623615369246010460810230373021899784471031262460139791812770652868643824890793643975640187107777935213576178260298550525385587924259812882071424357103045779073295852446950425491778"
              ],
              [
                "x-ray",
                "703747254237397915249820927690096013200431875897656778006106174585171654435330847039361311237550400897913352347946880617247329327584195785217361379013288435681390350754627669206610303409328842019936879962806363815660319627565772357683826395280759052264369664805474219568624809982935301688511968717269578225138372783398908274382799385068239773894812818078533316555793439759884749446165487205046831486339427120960312430456306126302629669292805945659166504953580456312176279130088083340901093653356234926030432589945536087247211432976603460210090174317819601382480288427059212367025188898143557140816523731764080712312171758067750869515512338317317995574070231770526262596313302450474804047877240"
              ],
              [
                "age",
                "397034117901722451269908176347570120723206352830828481384334662605661568698557277385928002298942434691666021722209104022519524243530967758432704518338387392454605853554255120038261834391819481484135948905861791707600809921110093625770946762283583715824717792698806660924178210955559404686505560176002012319450912913222327181443147219095337674849802495485282558705536974982709439782785673752212658680745277553331301741930743808194333551865168377199709984031374842087678432998361114778668212774118581321623417722705362830405239453677004261150641198837940214272537364167040605552440489538347940224758622514837375165618673627591721798065887020061995202329155451578965237709994651970834051450848184"
              ],
              [
                "name",
                "371396510210603803939360656879407816960442430715589993463818928088482154659104126872323248335275064099105734067971464259159389753663143567074103361229356051472459110483170587218982871316046300655247291373206326445576481407598051915944871053878616088089864321666502730401634653364078028517815004433388077054459747356414450305791374776209862232741972045838443877110194665080573869781574775736931285480978233932342958763116913203642216360461791183434633190385230572795922813490122227590436836928666039757961793936341409339498449911836606788108188855345417789161058755603327405513071960191375478365137605020233594497789029077779411702506341693997966044795128922272482003641170191929156055272863027"
              ]
            ]
          },
          "nonce": "457012367872739885200579"
        }
      },
      "request": {
        "indy": {
          "prover_did": "XtS7WeBqWnS1gSADjiyWkn",
          "cred_def_id": "TL1EaPFCZ8Si5aUrqScBDt:3:CL:2490:default",
          "blinded_ms": {
            "u": "90600261702604838909017276385304666802080026434152582629497066875984873624473586016944894811974546087727153555898007438310461862238433123340882673192645133813601220169721420829573578595937132764329027053688110435202053361410115397412413746862861348112977547378621667044550764272629032125808460405192298914179749301539558870005556499531192304701941344527939526896782174745120800291659057600415127766554334676712372023920811975653886723662697248574094215468593725555681889264499664010105154719164584197238656758300646157489387461968569285705614979932009970704378484650950667528688872116218682516981562891786488086963357",
            "ur": null,
            "hidden_attributes": [
              "master_secret"
            ],
            "committed_attributes": {}
          },
          "blinded_ms_correctness_proof": {
            "c": "43098503587336237755967828136081243791130516865882219214359075296351973112970",
            "v_dash_cap": "899809288446630813458775603179337557832305799048900389517162269254069838643602595296952020268649970128472030759278003968467192421648001480991086190803476422690708177632055679066490603163324113826402964743309940303182019128249357051696725165462966845816508385417397772980679373309982538378810554178931987719962761952815064600330435520358895503696551790740487413128239840664459105750240370209408143584702964077144047948762437065208080130783474737388605175299296204447137282983847417082505677061553726350511887769158431816121334276287465215171159774846816640311261611858422493158066435779635882968743444112683067169554327760047705687536112264230340350629443709970388940277613167124548560197821982058946365901228654837922",
            "m_caps": {
              "master_secret": "5830726796287030912173000629022008710520786216377121630973563316859371145313565612110663664865647816183975285628679981010455280981672086772155676017211154008249502006918152868730"
            },
            "r_caps": {}
          },
          "nonce": "754703732426017707636524"
        }
      },
      "credential": {
        "indy": {
          "schema_id": "TL1EaPFCZ8Si5aUrqScBDt:2:schema-720e72db-658d-49a7-bb0f-df5b8f06e53f:1.0",
          "cred_def_id": "TL1EaPFCZ8Si5aUrqScBDt:3:CL:2490:default",
          "rev_reg_id": null,
          "values": {
            "name": {
              "raw": "John",
              "encoded": "76355713903561865866741292988746191972523015098789458240077478826513114743258"
            },
            "x-ray": {
              "raw": "some x-ray",
              "encoded": "43715611391396952879378357808399363551139229809726238083934532929974486114650"
            },
            "age": {
              "raw": "99",
              "encoded": "99"
            },
            "profile_picture": {
              "raw": "profile picture",
              "encoded": "28661874965215723474150257281172102867522547934697168414362313592277831163345"
            }
          },
          "signature": {
            "p_credential": {
              "m_2": "19989617328717447475953868269643526851552739765627952100052387905609496644774",
              "a": "34839074650477682623274150572727580712657960790756921831152286748389939227065515171484237096673183204633231264636567725150671360829695505888657569992758871010773030148415526854813792584409060339343346706682238593722163687072565353331265961271146005423135741105154185464033105607075991425431556836647012276629640157485796487589265737549773917127318686444689073017222121124466525105158527705700858264068403700869301910241470392652311319265522584843630862150169658130841540815737982603334564765050775858241232917079967920290009984892377941599154859394353901416040461562193400911293615399469225500488126961585019914102382",
              "e": "259344723055062059907025491480697571938277889515152306249728583105665800713306759149981690559193987143012367913206299323899696942213235956742929684589612820703790461153203896563761",
              "v": "10019413052200911482302288267118717151752494712204732312580003757580042116312706555234151416014679710729196629215014638492013038396782058345074299373562230043116570009096708015703064528021423174867088794446999610999888273160546179691518189686534786632545489247431006985962650440046353619059113805278273237711816126329425631352489623214753954598648879828192242409321026618789422856402235381612652238543438652283940061192463260501824289419240500746100060054548922245366305780647421675975190633712412156268366173872284735570933487225370405886031944147740453800106514565421429561256011722765925328381507763000372684181921668528694774976278797440957345119262905509913255059494823475291742892596996528223962985516917115004003980009398361400623236911767484006094297590492985907474305232672496552623722760578806900684088497391642"
            },
            "r_credential": null
          },
          "signature_correctness_proof": {
            "se": "16853529904840453213815595948955439801805575983446975226801015107297202653202738340333381303662711024846588581400799220890004400210462747324158702254711104809008962673932001483340480415797527467728248089850979439551350903422425442701080088430246088748647533000558638352746875448600052187065442294119909012134365762448770090876739438176159847194349019117664800036272454277095339336666168139246808303463660767817487350937821345210942331229188432662011629404774108554127600574609544485826719864078464153606233151462396687199200410311893534452706320035899945007508336524405074876902460221692788021907268486350267252225963",
            "c": "45836158381769022817874176072126957336788480826575803229215272598856388805205"
          },
          "rev_reg": null,
          "witness": null
        }
      }
    }
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 16:54:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/876" class=".btn">#876</a>
            </td>
            <td>
                <b>
                    chore: update with main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 14:26:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/873" class=".btn">#873</a>
            </td>
            <td>
                <b>
                    build!: remove support for node 12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                wip - needs testing

Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 12:45:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/872" class=".btn">#872</a>
            </td>
            <td>
                <b>
                    docs: accessing rust logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 12:09:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/871" class=".btn">#871</a>
            </td>
            <td>
                <b>
                    docs: update developer readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                adds some hints for debugging running tests

Signed-off-by: Moriarty <moritz@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 10:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/870" class=".btn">#870</a>
            </td>
            <td>
                <b>
                    feat(credentials): delete associated didCommMessages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Moriarty <moritz@animo.id>

closes #728 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 10:15:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/869" class=".btn">#869</a>
            </td>
            <td>
                <b>
                    Mjrmergemain ppv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 07:42:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    fix(credentials): store revocation identifiers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #863 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 13:37:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/862" class=".btn">#862</a>
            </td>
            <td>
                <b>
                    fix(credentials): indy cred attachment format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 10:43:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/861" class=".btn">#861</a>
            </td>
            <td>
                <b>
                    fix(credentials): parse and validate preview @type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 10:25:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/857" class=".btn">#857</a>
            </td>
            <td>
                <b>
                    fix(node): only send 500 if no headers sent yet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If an error occurred after a message has been sent in response in the http inbound transport it would error out because we can't return a response twice in http. This just checks if the response is already sent
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:56:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/856" class=".btn">#856</a>
            </td>
            <td>
                <b>
                    fix(credentials): use interface in module api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                My previous PR to generalize the crdentials module undid some of the changes to only allow interfaces.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:45:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/855" class=".btn">#855</a>
            </td>
            <td>
                <b>
                    fix(credentials): proposal preview attribute 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the v2 preview `credential_proposal` should be `credential_preview`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:06:28 +0000 UTC
    </div>
</div>

