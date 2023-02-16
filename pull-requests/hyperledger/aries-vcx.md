---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/755" class=".btn">#755</a>
            </td>
            <td>
                <b>
                    Add tests on top of messages_crate PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                First iteration, needed to get my hands on. Feel free to merge OR close and just cherry-pick useful parts if your local revision is perhaps already ahead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 22:22:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/754" class=".btn">#754</a>
            </td>
            <td>
                <b>
                    Refactor/messages crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor of messages crate.

Planned steps:
  - Initially, development will be carried in a new crate, `messages2`.
  - After the crate is complete, it's integration will be done within `aries_vcx`.
 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 23:40:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/752" class=".btn">#752</a>
            </td>
            <td>
                <b>
                    Rename connection 'Complete' state to 'Completed'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - We are using past tense form to name protocol states, for example `Requested`, `Finished`, `Sent`, except for Connection's `Complete` state. This PR unifies the naming, renaming `Complete -> Completed`
- Mediated Connection note: although it's discouraged to rely on the serialized form of state machines, note that mediated connection even previously serialized `Complete` state as `"Completed"`, so this does not present any practical change for mediated connection, but purely internal. 

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 13:21:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/751" class=".btn">#751</a>
            </td>
            <td>
                <b>
                    Update CI host images to ubuntu 22.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 15:56:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/750" class=".btn">#750</a>
            </td>
            <td>
                <b>
                    Fix NodeJS testing CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span>
            </td>
            <td>
                NodeJS CI testing changes:
- upgrade host machines to ubuntu 22.04
- run only against nodejs 18, drop 12
- downgrade npm from default `9.x` to `8.x` instead (on 9x, npm can't resolve `@hyperledger/vcx-napi-rs-linux-x64-gnu` from `node-wrapper`; for example: https://github.com/hyperledger/aries-vcx/actions/runs/4166607529/jobs/7211161331)

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 14:01:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/749" class=".btn">#749</a>
            </td>
            <td>
                <b>
                    Simplify connection serialization from nodejs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span><span class="chip">skip-napi-m1</span>
            </td>
            <td>
                - NodeJS wrapper was previously trying to keep value of `source_id` as part of constructed JS objects / TS classes, see changes in class `VcxBase`
```
protected _sourceId: string;
```
- Consequently deserialization constructors requiring `source_id`. That led me to generalizing signature for its static method ` _deserialize` such the serialized data to be deserialized are simply a JSON object (expressed as `Record<string, unknown>` in TS) instead of previous more strict definition `objData: ISerializedData<{ source_id: string }>`  which couldn't acommodate different serialization format of `Connection` state machine.
- Additionally removed some dead code
- Note: More code can be purged and cleaned up, for example given the decision to treat serialized data as opaque, it makes no sense to define `ISerializedData`, as this is expression of certain assumption as to how that serialized data looks like. The only thing which should be held by TS classes is the numeric rust handle
- Simplifies `Connection` serialization such that in serialized to (removing extra `data` level in hierarchy, removes duplicated field `source_id`, removes `version`)
```
{
    "source_id": "",
    "pairwise_info": {
        "pw_did": "FhrSrYtQcw3p9xwf7NYemf",
        "pw_vk": "91qMFrZjXDoi2Vc8Mm14Ys112tEZdDegBZZoembFEATE"
    },
    "state": {
        "Inviter": {
            "Initial": null
        }
    }
}
```



Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 11:37:47 +0000 UTC
    </div>
</div>

