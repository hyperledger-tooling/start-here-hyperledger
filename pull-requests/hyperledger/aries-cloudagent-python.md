---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2175" class=".btn">#2175</a>
            </td>
            <td>
                <b>
                    Pass document loader to jsonld.expand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes test cases where the JSON-LD context was being downloaded erroneously, and probably speeds up the tests. The following tests failed previously while the BBS security context was unavailable.

```FAILED aries_cloudagent/protocols/present_proof/dif/tests/test_pres_exch_handler.py::TestPresExchHandler::test_limit_disclosure_required_check
FAILED aries_cloudagent/protocols/present_proof/dif/tests/test_pres_exch_handler.py::TestPresExchHandler::test_create_vc_record_with_graph_struct
FAILED aries_cloudagent/protocols/present_proof/dif/tests/test_pres_exch_handler.py::TestPresExchHandler::test_derive_cred_missing_credsubjectid
FAILED aries_cloudagent/protocols/present_proof/dif/tests/test_pres_exch_handler.py::TestPresExchHandler::test_derive_cred_credsubjectid
FAILED aries_cloudagent/protocols/present_proof/dif/tests/test_pres_exch_handler.py::TestPresExchHandler::test_derive_nested_cred_missing_credsubjectid_a
FAILED aries_cloudagent/protocols/present_proof/dif/tests/test_pres_exch_handler.py::TestPresExchHandler::test_derive_nested_cred_missing_credsubjectid_b
FAILED aries_cloudagent/protocols/present_proof/dif/tests/test_pres_exch_handler.py::TestPresExchHandler::test_derive_nested_cred_credsubjectid
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_a
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_b
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_c
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_limit_disclosure_fail_a
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_limit_disclosure_fail_b
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_no_match_a
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_no_match_b
FAILED aries_cloudagent/protocols/present_proof/v2_0/formats/dif/tests/test_handler.py::TestDIFFormatHandler::test_verify_received_pres_sequence
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 22:07:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2174" class=".btn">#2174</a>
            </td>
            <td>
                <b>
                    WIP: Peer DID Method 1
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
        Created At 2023-03-21 14:48:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2173" class=".btn">#2173</a>
            </td>
            <td>
                <b>
                    Add support for JsonWebKey2020 for the connection invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added support for the JsonWebKey2020 OKP keys for connection invitations.
To avoid extensive refactoring this is done by converting it to the supported base58 format.

Please, give feedback.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-21 09:37:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2170" class=".btn">#2170</a>
            </td>
            <td>
                <b>
                    BREAKING: feat: get queued outbound message in transport handle message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will enable queues to annotate outbound messages with relevant context for things like dead letter queues that know which wallet sent the message that failed, what message was being sent, etc.

This is a breaking change for plugins adding queue implementations (cc @shaangill025) but we think this is worthwhile for the ability to improve internal error handling.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 14:52:14 +0000 UTC
    </div>
</div>

