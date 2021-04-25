---
layout: default
title: fabric-sdk-py
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/fabric-sdk-py
---

# fabric-sdk-py <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-py){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric-sdk-py/issues/137" class=".btn">137</a>
            </td>
            <td>
                <b>
                    fix rl-report issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Priority: Medium</span><span class="chip">Type: Enhancement</span><span class="chip">help wanted</span>
            </td>
            <td>
                The report is [here](https://github.com/ryjones/rl-report/blob/main/main/fabric-sdk-py-repolinter-report.md). We can add some files to fix the raised issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-03-25 03:37:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric-sdk-py/issues/135" class=".btn">135</a>
            </td>
            <td>
                <b>
                    Problem creating channel in python tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Priority: Medium</span><span class="chip">Type: Question</span><span class="chip">help wanted</span><span class="chip">starter</span>
            </td>
            <td>
                Hello. I am having trouble running the python sdk example to create a channel with the default values. I have already added the binaries to my path, etc. 

This is the code I am running within the fabric-sdk-py folder:
import asyncio
from hfc.fabric import Client
loop = asyncio.get_event_loop()

cli = Client(net_profile="test/fixtures/network.json")
print(cli.organizations)  # orgs in the network
print(cli.peers)  # peers in the network
print(cli.orderers)  # orderers in the network
print(cli.CAs)  # ca nodes in the network

org1_admin = cli.get_user(org_name='org1.example.com', name='Admin')

# Create a New Channel, the response should be true if succeed
response = loop.run_until_complete(cli.channel_create(
            orderer='orderer.example.com',
            channel_name='businesschannel',
            requestor=org1_admin,
            config_yaml='test/fixtures/e2e_cli/',
            channel_profile='TwoOrgsChannel'
            ))
print(response == True)

And the error I am getting is:
Init client with profile=test/fixtures/network.json
create org with name=orderer.example.com
create org with name=org1.example.com
create org with name=org2.example.com
create ca with name=ca-org1
create ca with name=ca-org2
Import orderers = dict_keys(['orderer.example.com'])
Import peers = dict_keys(['peer0.org1.example.com', 'peer1.org1.example.com', 'peer0.org2.example.com', 'peer1.org2.example.com'])
{'orderer.example.com': <hfc.fabric.organization.Organization object at 0x7f7d1a9d9a60>, 'org1.example.com': <hfc.fabric.organization.Organization object at 0x7f7d1cebadf0>, 'org2.example.com': <hfc.fabric.organization.Organization object at 0x7f7d1ced5e50>}
{'peer0.org1.example.com': <hfc.fabric.peer.Peer object at 0x7f7d1ced5760>, 'peer1.org1.example.com': <hfc.fabric.peer.Peer object at 0x7f7d1ced5280>, 'peer0.org2.example.com': <hfc.fabric.peer.Peer object at 0x7f7d1ced5eb0>, 'peer1.org2.example.com': <hfc.fabric.peer.Peer object at 0x7f7d1a68c790>}
{'orderer.example.com': <hfc.fabric.orderer.Orderer object at 0x7f7d1ced56a0>}
{'ca-org1': <hfc.fabric.certificateAuthority.certificateAuthority object at 0x7f7d1ced5d60>, 'ca-org2': <hfc.fabric.certificateAuthority.certificateAuthority object at 0x7f7d1ced5a60>}
FABRIC_CFG_PATH set to /home/hoovert/fabric-sdk-py/test/fixtures/e2e_cli/
--- Logging error ---
Traceback (most recent call last):
  File "/usr/local/lib/python3.9/logging/__init__.py", line 1079, in emit
    msg = self.format(record)
  File "/usr/local/lib/python3.9/logging/__init__.py", line 923, in format
    return fmt.format(record)
  File "/usr/local/lib/python3.9/logging/__init__.py", line 659, in format
    record.message = record.getMessage()
  File "/usr/local/lib/python3.9/logging/__init__.py", line 363, in getMessage
    msg = msg % self.args
TypeError: not all arguments converted during string formatting
Call stack:
  File "/home/hoovert/fabric-sdk-py/test1.py", line 16, in <module>
    response = loop.run_until_complete(cli.channel_create(
  File "/usr/local/lib/python3.9/asyncio/base_events.py", line 629, in run_until_complete
    self.run_forever()
  File "/usr/local/lib/python3.9/asyncio/base_events.py", line 596, in run_forever
    self._run_once()
  File "/usr/local/lib/python3.9/asyncio/base_events.py", line 1890, in _run_once
    handle._run()
  File "/usr/local/lib/python3.9/asyncio/events.py", line 80, in _run
    self._context.run(self._callback, *self._args)
  File "/home/hoovert/fabric-sdk-py/hfc/fabric/client.py", line 505, in channel_create
    tx = self.generate_channel_tx(channel_name, config_yaml,
  File "/home/hoovert/fabric-sdk-py/hfc/fabric/client.py", line 1117, in generate_channel_tx
    _logger.error('Failed to generate transaction file', err)
Message: 'Failed to generate transaction file'
Arguments: (b'\x1b[34m2021-02-23 16:39:18.006 -05 [common.tools.configtxgen] main -> INFO 001\x1b[0m Loading configuration\n\x1b[34m2021-02-23 16:39:18.010 -05 [common.tools.configtxgen.localconfig] Load -> INFO 002\x1b[0m Loaded configuration: /home/hoovert/fabric-sdk-py/test/fixtures/e2e_cli/configtx.yaml\n\x1b[34m2021-02-23 16:39:18.010 -05 [common.tools.configtxgen] doOutputChannelCreateTx -> INFO 003\x1b[0m Generating new channel configtx\n\x1b[35m2021-02-23 16:39:18.010 -05 [common.tools.configtxgen] main -> FATA 004\x1b[0m Error on outputChannelCreateTx: could not generate default config template: error parsing configuration: error adding policies to channel group: no policies defined\n',)
Configtx is empty
False

Any help greatly appreciated. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-02-23 21:44:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric-sdk-py/issues/134" class=".btn">134</a>
            </td>
            <td>
                <b>
                    enroll admin error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Priority: Medium</span><span class="chip">Type: Bug</span><span class="chip">Type: Question</span><span class="chip">help wanted</span>
            </td>
            <td>
                Hi, all!

I set all the environment locally and run the fabcar example in fabric_sample. 
downloaded this python version sdk, run : adminEnrollment = casvc.enroll("admin","adminpw") 

the error shows like: json.decoder.JSONDecodeError expecting value: line 1 column 1 (char 0)

I was blocked by this error for 2 days, if anyone knows why just let me know,  thank you in advance!


Init client with profile=test/fixtures/network.json
create org with name=orderer.example.com
create org with name=org1.example.com
create org with name=org2.example.com
create ca with name=ca-org1
create ca with name=ca-org2
Import orderers = dict_keys(['orderer.example.com'])
Import peers = dict_keys(['peer0.org1.example.com', 'peer1.org1.example.com', 'peer0.org2.example.com', 'peer1.org2.example.com'])
Traceback (most recent call last):
  File "lr.py", line 61, in <module>
    adminEnrollment = casvc.enroll("admin","adminpw") # now local will have the admin enrollment
  File "/home/yusen/Desktop/fabric-sdk-py/hfc/fabric_ca/caservice.py", line 484, in enroll
    enrollmentCert, caCertChain = self._ca_client.enroll(
  File "/home/yusen/Desktop/fabric-sdk-py/hfc/fabric_ca/caservice.py", line 328, in enroll
    res, st = self._send_ca_post(path='enroll',
  File "/home/yusen/Desktop/fabric-sdk-py/hfc/fabric_ca/caservice.py", line 255, in _send_ca_post
    return r.json(), r.status_code
  File "/home/yusen/anaconda3/lib/python3.8/site-packages/requests/models.py", line 889, in json
    return complexjson.loads(
  File "/home/yusen/anaconda3/lib/python3.8/json/__init__.py", line 357, in loads
    return _default_decoder.decode(s)
  File "/home/yusen/anaconda3/lib/python3.8/json/decoder.py", line 337, in decode
    obj, end = self.raw_decode(s, idx=_w(s, 0).end())
  File "/home/yusen/anaconda3/lib/python3.8/json/decoder.py", line 355, in raw_decode
    raise JSONDecodeError("Expecting value", s, err.value) from None
**json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)**

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-02-05 06:42:02 +0000 UTC
    </div>
</div>

