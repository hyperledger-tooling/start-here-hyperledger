---
layout: default
title: firefly-fabconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    README.md and .gitignore small improvement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jan Rock <jan.rock@me.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 21:20:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Identity support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note: not focusing on tests right now so that the FireFly integration can proceed sooner, which is an important exercise to inform the architectural validation to accommodate multiple ledger technologies

## Create (register)
```
$ curl -H "Content-Type: application/json" -d '{"name":"user102","type":"client"}' http://localhost:3000/identities | jq
{
  "name": "user102",
  "secret": "nzzoCYRTxaRj"
}
```

including error handling:
```
$ curl -H "Content-Type: application/json" -d '{"name":"user102","type":"client"}' http://localhost:3000/identities | jq
{
  "error": "failed to register user: failed to register user: Response from server: Error Code: 0 - Registration of 'user102' failed: Identity 'user102' is already registered\n"
}
```

## Enroll
```
$ curl -H "Content-Type: application/json" -d '{"secret":"nzzoCYRTxaRj"}' http://localhost:3000/identities/user102/enroll 
{
  "name": "",
  "success": true
}
```

## List
```
g$ curl http://localhost:3000/identities | jq
[
  {
    "name": "admin",
    "maxEnrollments": -1,
    "type": "client",
    "affiliation": "",
    "caname": ""
  },
  {
    "name": "u0cr3kb8sl",
    "maxEnrollments": 1,
    "type": "orderer",
    "affiliation": "",
    "caname": ""
  },
  {
    "name": "u0cr3kb8sl-admin",
    "maxEnrollments": 1,
    "type": "admin",
    "affiliation": "",
    "caname": ""
  },
```

## Get
```
$ curl http://localhost:3000/identities/user102 | jq
{
  "name": "user102",
  "maxEnrollments": -1,
  "type": "client",
  "affiliation": "",
  "caname": "u0vgwu9s00"
}
```

## Using a newly registered and enrolled signing identity to submit transactions
```
$ curl -H "Content-Type: application/json" -d '{"headers":{"type":"SendTransaction","channel":"default-channel","signer":"user102"},"chaincode":"asset_transfer","func":"CreateAsset","args":["asset1016","yellow","10","Tom","1300"]}' http://localhost:3000/transactions | jq
{
  "sent": true,
  "id": "1621fcad-d42e-4489-7956-2d056901850c"
}

[2021-07-29T18:28:15.316-04:00]  INFO --> POST /transactions
[2021-07-29T18:28:15.316-04:00]  INFO Request handler accepted message. MsgID: 1621fcad-d42e-4489-7956-2d056901850c Type: SendTransaction
[2021-07-29T18:28:15.316-04:00]  INFO In-flight 1000001 added. signer=user102 before=0
[2021-07-29T18:28:15.316-04:00]  INFO <-- POST /transactions [202]:
{"sent":true,"id":"1621fcad-d42e-4489-7956-2d056901850c"}
[2021-07-29T18:28:16.068-04:00]  INFO TX: Sent OK [0.75s]
[2021-07-29T18:28:16.170-04:00]  INFO Obtained receipt after 101.97ms - average time to receipt: 101.97ms
[2021-07-29T18:28:16.170-04:00]  INFO Receipt for f39a3c720c8013b654527258332d05c5ea341e05939e2f42d7516554ee74fb9c obtained after 0.10s Success=true
[2021-07-29T18:28:16.170-04:00]  INFO Received reply message. requestId='1621fcad-d42e-4489-7956-2d056901850c' reqOffset='' type='TransactionSuccess': 
[2021-07-29T18:28:16.171-04:00]  INFO 1621fcad-d42e-4489-7956-2d056901850c: Inserted receipt into receipt store
[2021-07-29T18:28:16.171-04:00]  INFO In-flight 1000001 complete. signer=user102 sub=true before=1 after=0
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-30 13:06:51 +0000 UTC
    </div>
</div>

