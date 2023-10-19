---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    add tokengen function to update auditor and issuer certs in dlog pp files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the auditor or issuer certificate expires, we have to update it in the token chaincode. This action should *not* change the public parameters, because this would render existing tokens/proofs invalid.

This PR adds a command to the tokengen cli utility to update the auditor and/or issuers certificates in an existing `zkatdlog_pp.json`, without changing the public parameters.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 14:13:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    use latest idemix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 09:20:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/506" class=".btn">#506</a>
            </td>
            <td>
                <b>
                    use fsc logger for badger database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                Badger has noisy logs when writing:

```
badger 2023/10/14 14:23:14 INFO: Sent range 21 for iteration: [74720030326639616465313833666639626134363335393737663132626663346364623435333331393839383331323261316135316365383262353663666563313961ffffffffffffffcc, 74720030336166653834326463653735376631373764346131393034656433623436313863323964613630666632383561663537623363613462356437333232613836fffffffffffffffb) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 22 for iteration: [74720065353032323934376132623034663538646431336139373930336430346439336338313935366162653061613463636262333934376663396263663061316435ffffffffffffffdb, 74720066303236363664653166373534643461316234313133613433646162356266333566366662373339326665343466336234656137643464393262663130393631ffffffffffffffdf) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 23 for iteration: [74720062303332613234356530323032346232336434616361303934343439376162386632373766386534613834656537623934626336333566643837643236396632ffffffffffffffe6, 74720063373963346161323736366464376132356539313364333833633665613762386133313538396431316139616137663632333336353338306536393262643736fffffffffffffff1) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 24 for iteration: [74720066373264366464643866636164383063373237643762623063666632366335323630373434393966353631373464663836373538353332656438313432303036ffffffffffffffd9, 74720066626433353233383935346234656333343766636430376465303036633763656264393333313232393736616432626339336466646133626132346361313164ffffffffffffffdd) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 25 for iteration: [74720066626433353233383935346234656333343766636430376465303036633763656264393333313232393736616432626339336466646133626132346361313164ffffffffffffffdd, 74720066643039626431663435636336383637343333366138643134396166663837363837653639613337333232613466623266386532386432343433653732333637ffffffffffffffd3) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 26 for iteration: [74720066643039626431663435636336383637343333366138643134396166663837363837653639613337333232613466623266386532386432343433653732333637ffffffffffffffd3, 74780061616161616161616161616161616161616161616161616161610036323038326361613166373232343633623834343737366630623338326361643630313430353431656463353764336333366638666338643231316465353838fffffffffffffffc) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 27 for iteration: [6964736571ffffffffffffffe7, 74720030303138346335323166643862626532366566383239303263373630326163653761383666353562303134636439366236363934356335646135663538343232ffffffffffffffd5) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 28 for iteration: [74780061616161616161616161616161616161616161616161616165630030303138346335323166643862626532366566383239303263373630326163653761383666353562303134636439366236363934356335646135663538343232ffffffffffffffd4, ) of size: 706 KiB
badger 2023/10/14 14:23:14 INFO: ttxdb.SetStatus Sent data of size 40 KiB
```

The output couldn't be controlled, because the badger was being initiated with default options including the default golang logger. 

This PR injects the FSC logger into the badger config, so that the format corresponds to the rest of the logs of the Token SDK and can be controlled via the logging.spec config key (example: `info,token-sdk.ttxdb.badger=warn` will keep 'info' as the standard level, but get rid of the noisy badger logs).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-14 12:49:57 +0000 UTC
    </div>
</div>

