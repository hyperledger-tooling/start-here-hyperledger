---
layout: default
title: firefly-perf-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-perf-cli
---

# firefly-perf-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-perf-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Consistent readahead
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
        Created At 2023-06-01 15:36:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Adding clean up logic for listeners and subscriptions for each run
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                as per title
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 13:58:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-perf-cli/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    Manual endpoints skipped config from instances
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found that the test runner for "manual endpoint" configurations, did not pick up mandatory config from the `instances` array.

The error was as follows, so I had to add some debug first (to get it to report the error from FireFly, rather than assuming a HTTP OK response):

```
panic: interface conversion: interface {} is nil, not string

goroutine 1 [running]:
github.com/hyperledger/firefly-perf-cli/internal/perf.(*perfRunner).createEthereumContractListener(0xc0000bfc00, {0xc000026240, 0x37})
	/home/ubuntu/test-dtcc-kap/firefly-perf-cli/internal/perf/perf.go:969 +0x690
github.com/hyperledger/firefly-perf-cli/internal/perf.(*perfRunner).Start(0xc0000bfc00)
	/home/ubuntu/test-dtcc-kap/firefly-perf-cli/internal/perf/perf.go:284 +0x347
github.com/hyperledger/firefly-perf-cli/cmd.glob..func2(0x1021520, {0xad09fb, 0x4, 0x4})
	/home/ubuntu/test-dtcc-kap/firefly-perf-cli/cmd/run.go:89 +0x93
github.com/spf13/cobra.(*Command).execute(0x1021520, {0xc00006c140, 0x4, 0x4})
	/home/ubuntu/go/pkg/mod/github.com/spf13/cobra@v1.6.1/command.go:916 +0x842
github.com/spf13/cobra.(*Command).ExecuteC(0x1021240)
	/home/ubuntu/go/pkg/mod/github.com/spf13/cobra@v1.6.1/command.go:1044 +0x3cd
github.com/spf13/cobra.(*Command).Execute(...)
	/home/ubuntu/go/pkg/mod/github.com/spf13/cobra@v1.6.1/command.go:968
github.com/hyperledger/firefly-perf-cli/cmd.Execute()
	/home/ubuntu/test-dtcc-kap/firefly-perf-cli/cmd/root.go:64 +0x25
main.main()
	/home/ubuntu/test-dtcc-kap/firefly-perf-cli/ffperf/main.go:26 +0x19
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 19:17:36 +0000 UTC
    </div>
</div>

