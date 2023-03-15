---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Add apiclient command line tools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new `apiclient` package with an `FFTMClient` interface (and implementation). This allows any blockchain connector to also act as an API client by adding a single line of code to enable its executable like this:

```diff
func init() {
	rootCmd.PersistentFlags().StringVarP(&cfgFile, "config", "f", "", "config file")
	rootCmd.AddCommand(versionCommand())
	rootCmd.AddCommand(configCommand())
+	rootCmd.AddCommand(fftmcmd.ClientCommand())
}
```

This then allows an operator to invoke the blockchain connector binary to run various client commands such as:

```
./firefly-evmconnect client eventstreams list --url http://127.0.0.1:5102
[
  {
    "id": "0186c1c2-4aa6-98e4-8df2-702e552e7174",
    "created": "2023-03-08T15:06:21.222375209Z",
    "updated": "2023-03-08T15:06:21.222375209Z",
    "name": "0",
    "suspended": false,
    "type": "websocket",
    "errorHandling": "block",
    "batchSize": 50,
    "batchTimeout": "500ms",
    "retryTimeout": "30s",
    "blockedRetryDelay": "30s",
    "websocket": {
      "distributionMode": "load_balance"
    }
  }
]
```

This PR is not meant to be a comprehensive CLI implementation, but contains the foundation for building additional commands, as well as a few useful utilities. The current list of implemented functions can be found in the `FFTMClient` interface:

```go
type FFTMClient interface {
	GetEventStreams(ctx context.Context) ([]apitypes.EventStream, error)
	GetListeners(ctx context.Context, eventStreamID string) ([]apitypes.Listener, error)
	DeleteEventStream(ctx context.Context, eventStreamID string) error
	DeleteEventStreamsByName(ctx context.Context, nameRegex string) error
	DeleteListener(ctx context.Context, eventStreamID, listenerID string) error
	DeleteListenersByName(ctx context.Context, eventStreamID, nameRegex string) error
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 18:22:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    update readme for tranaction handler refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Readme update for tranaction handler refactor

for #57 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 14:18:50 +0000 UTC
    </div>
</div>

