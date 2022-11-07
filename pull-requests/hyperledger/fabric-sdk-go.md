---
layout: default
title: fabric-sdk-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-go
---

# fabric-sdk-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    Supports loading of config values for Orderer.Endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fabric version: [release-2.2](https://github.com/hyperledger/fabric/tree/release-2.2)

configtx.yaml(release-2.2): [configtx.yaml](https://github.com/hyperledger/fabric-samples/blob/v2.2.0/test-network/configtx/configtx.yaml)

sdk_config file : [config_e2e.yaml](https://github.com/hyperledger/fabric-sdk-go/blob/main/test/fixtures/config/config_e2e.yaml) without `certificateAuthorities` config

When I call the chaincode transaction using the code below, fabric-sdk-go returns 'orderers is nil'. I found out that this is due to the channel configuration of the application channel with Orderer.Endpoints but not OrdererAddresses, and the loadConfigValue function does not support "Endpoints" configuration loading.

```golang
func main() {
	sdk, err := fabsdk.New(config.FromFile("config_e2e.yaml"))
	if err != nil {
		log.Fatalln(err)
	}
	defer sdk.Close()
	cli, err := channel.New(sdk.ChannelContext("mychannel", fabsdk.WithUser("Admin"), fabsdk.WithOrg("Org1"),
	))
	if err != nil {
		log.Fatalln(err)
	}
	resp, err := cli.Execute(channel.Request{
		ChaincodeID: "abstore",
		Fcn:         "init",
		Args:        [][]byte{[]byte("a"), []byte("100"), []byte("b"), []byte("200")},
		IsInit:      true,
	})
	if err != nil {
		log.Fatalln(err)
	}
	log.Println(string(resp.TransactionID))
}
```

Signed-off-by: smallsixFight smallsix.fight@gmail.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 03:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-go/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    Add transient map support for the gateway client
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
        Created At 2022-11-04 18:50:47 +0000 UTC
    </div>
</div>

