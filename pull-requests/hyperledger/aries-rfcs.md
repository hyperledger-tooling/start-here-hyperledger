---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/740" class=".btn">#740</a>
            </td>
            <td>
                <b>
                    README.md of Overlays Capture Architecture (OCA) : RFC 0013
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated the Author affiliation to The Human Colossus Foundation;
- Updated the architecture name to Overlays Capture Architecture (OCA).

Signed-off-by: Paul Knowles <44690468+pknowl@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 15:06:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/739" class=".btn">#739</a>
            </td>
            <td>
                <b>
                    Update AIP 2.0 link commit references to reflect recent clarifications to RFC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the AIP 2 RFC links to specific commits to add in clarifications made since AIP 2.0 was last updated (March 2022). The additions are listed here, with the full "diff" output listed lower in this note:

* Adds a changelog section to AIP 2.0 to note when clarification link updates are made and to what RFCs
* RFC 0023 DID Exchange - adds clarification on the use of label and goal_codes in DID Exchange messages.
* RFC 0025 DIDComm Transports - adds clarification that when using HTTP transport, HTTPS is generally necessary whenever a mobile OS is involved.
* RFC 0434 Out of Band - clarification on the use of Base64URL encoding and in the use of redirection, and how some HTTP libraries automated the handling of redirects.

### Diffs of the update RFCs:

The following are the full set of clarification diffs for the RFC commits being changed:

```
>>>>>>>> Changed protocol: features/0023-did-exchange, latest commit to protocol: bf3d796cc33ce78ed7cde7f5422b10719a68be21

diff --git a/features/0023-did-exchange/README.md b/features/0023-did-exchange/README.md
index 583df63..213b962 100644
--- a/features/0023-did-exchange/README.md
+++ b/features/0023-did-exchange/README.md
@@ -173,7 +173,7 @@ The _requester_ may provision a new DID according to the DID method spec. For a
 * The [`~thread`](../../concepts/0008-message-id-and-threading/README.md#thread-object) decorator MUST be included:
   * It MUST include the ID of the parent thread (`pthid`) such that the `request` can be correlated to the corresponding (implicit or explicit) `invitation`. More on correlation [below](#correlating-requests-to-invitations).
   * It MAY include the `thid` property. This works according to the [`thid`](../../concepts/0008-message-id-and-threading/README.md#thread-id-thid) property in the thread decorator, meaning that if `thid` is not defined it is implicitly defined as the `@id` on the same `request` message.
-* The `label` attribute provides a suggested label for the DID being exchanged. This allows the user to tell multiple exchange requests apart. This is not a trusted attribute.
+* The `label` attribute provides a suggested label for the DID being exchanged. This allows the user to tell multiple exchange requests apart. This is not a trusted attribute. (See note on `label` below)
 * The `goal_code` (optional) is a self-attested code the receiver may want to display to the user or use in automatically deciding what to do with the request message. The goal code might be used particularly when the request is sent to a resolvable DID without reference to a specfic invitation.
 * The goal (optional) is a self-attested string that the receiver may want to display to the user about the context-specific goal of the request message.
 * The `did` attribute MUST be included. It indicates the DID being exchanged.
@@ -181,6 +181,9 @@ The _requester_ may provision a new DID according to the DID method spec. For a
   * If the `did` is resolvable (either an inline `peer:did` or a publicly resolvable DID), the `did_doc~attach` attribute should not be included.
   * If the DID is a `did:peer` DID, the DIDDoc must be as outlined in [RFC 0627 Static Peer DIDs](../0627-static-peer-dids/README.md).
 
+
+The `label` property was intended to be declared as an optional property, but was added to the RFC as a required property. If an agent wishes to not use a label in the request, an empty string (`""`) or the set value `Unspecified` may be used to indicate a non-value. This approach ensures existing AIP 2.0 implementations do not break.
+
 #### Correlating requests to invitations
 
 An invitation is presented in one of two forms:

>>>>>>>> Changed protocol: features/0025-didcomm-transports, latest commit to protocol: f39481e92ad1a10dbc499cd4931a08c3497cee3f

diff --git a/features/0025-didcomm-transports/README.md b/features/0025-didcomm-transports/README.md
index b88eaad..9b8da47 100644
--- a/features/0025-didcomm-transports/README.md
+++ b/features/0025-didcomm-transports/README.md
@@ -22,7 +22,13 @@ Standardized transport methods are detailed here.
 
 ### HTTP(S)
 
-HTTP(S) is the first transport for DID Communication that has received heavy attention.
+HTTP(S) is the first, and most used transport for DID Communication that has received heavy attention. 
+
+While it is recognized that all DIDComm messages are secured through strong encryption, making HTTPS somewhat redundant, it will likely cause issues with mobile clients because venders (Apple and Google) are limiting application access to the HTTP protocol. For example, on iOS 9 or above where [ATS])(https://developer.apple.com/documentation/bundleresources/information_property_list/nsapptransportsecurity) is in effect, any URLs using HTTP must have an exception hard coded in the application prior to uploading to the iTunes Store. This makes DIDComm unreliable as the agent initiating the the request provides an endpoint for communication that the mobile client must use. If the agent provides a URL using the HTTP protocol it will likely be unusable due to low level operating system limitations.
+
+As a best practice, when HTTP is used in situations where a mobile client (iOS or Android) may be involved it is highly recommended to use the HTTPS protocol, specifically TLS 1.2 or above. 
+
+Other important notes on the subject of using HTTP(S) include:
 
 - Messages are transported via HTTP POST.
 - The MIME Type for the POST request is `application/didcomm-envelope-enc`; see [RFC 0044: DIDComm File and MIME Types](../0044-didcomm-file-and-mime-types/README.md) for more details.
@@ -58,7 +64,7 @@ XMPP is an effective transport for incoming DID-Communication messages directly
 - Independent of cloud agents and routing agents, as messages arrive directly at the mobile agent.
 - Well suited for direct consumer-to-consumer SSI transactions, from one mobile agent directly to another mobile agent without any DID-Communication intermediaries.
 - Simple encapsulation of DIDcom messages, getting trust from the DIDcom Encryption Envelope.
-- Specified in [Aries RFC 0024: DIDCom-over-XMPP](https://github.com/hyperledger/aries-rfcs/tree/master/features/0024-didcomm-over-xmpp)
+- Specified in [Aries RFC 0024: DIDCom-over-XMPP](https://github.com/hyperledger/aries-rfcs/tree/main/features/0024-didcomm-over-xmpp)
 
 #### Known Implementations
 

>>>>>>>> Changed protocol: features/0434-outofband, latest commit to protocol: 2bc7db66d15a55d70ce5bd16b2513a853c9d5749

diff --git a/features/0434-outofband/README.md b/features/0434-outofband/README.md
index 60d2df2..c8ec720 100644
--- a/features/0434-outofband/README.md
+++ b/features/0434-outofband/README.md
@@ -6,7 +6,7 @@
 - Status Note: This RFC extracts the `invitation` messages from the [DID Exchange](../../features/0023-did-exchange/README.md) protocol (and perhaps [Connection](../../features/0160-connection-protocol/README.md)), and replaces the combined `present_proof/1.0/request` combined with the `~service` decorator to define an ephemeral (connection-less) challenge.
 - Supersedes: Invitation Message in [0160-Connections](https://github.com/hyperledger/aries-rfcs/blob/9b0aaa39df7e8bd434126c4b33c097aae78d65bf/features/0160-connection-protocol/README.md#0-invitation-to-connect) and Invitation Message in [0023-DID-Exchange](https://github.com/hyperledger/aries-rfcs/blob/9b0aaa39df7e8bd434126c4b33c097aae78d65bf/features/0023-did-exchange/README.md#0-invitation-to-exchange).
 - Start Date: 2020-03-01
-- Tags: [feature](/tags.md#feature), [protocol](/tags.md#protocol)
+- Tags: [feature](/tags.md#feature), [protocol](/tags.md#protocol), [test-anomaly](/tags.md#test-anomaly)
 - URI: `https://didcomm.org/out-of-band/%VER`
 
 ## Summary
@@ -248,13 +248,13 @@ The processing rules for the `services` block are:
 
 The attributes in the inline form parallel the attributes of a DID Document for increased meaning. The `recipientKeys` and `routingKeys` within the inline block decorator **MUST** be [`did:key` references](https://digitalbazaar.github.io/did-method-key/).
 
-As defined in the [DIDComm Cross Domain Messaging RFC](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0094-cross-domain-messaging), if `routingKeys` is present and non-empty, additional forwarding wrapping are necessary in the response message.
+As defined in the [DIDComm Cross Domain Messaging RFC](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0094-cross-domain-messaging), if `routingKeys` is present and non-empty, additional forwarding wrapping are necessary in the response message.
 
 When considering routing and options for out-of-band messages, keep in mind that the more detail in the message, the longer the URL will be and (if used) the more dense (and harder to scan) the QR code will be.
 
 ##### Service Endpoint
 
-The service endpoint used to transmit the response is either present in the out-of-band message or available in the DID Document of a presented DID. If the endpoint is itself a DID, the `serviceEndpoint` in the DIDDoc of the resolved DID **MUST** be a URI, and the `recipientKeys` **MUST** contain a single key. That key is appended to the end of the list of `routingKeys` for processing. For more information about message forwarding and routing, see [RFC 0094 Cross Domain Messaging](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0094-cross-domain-messaging).
+The service endpoint used to transmit the response is either present in the out-of-band message or available in the DID Document of a presented DID. If the endpoint is itself a DID, the `serviceEndpoint` in the DIDDoc of the resolved DID **MUST** be a URI, and the `recipientKeys` **MUST** contain a single key. That key is appended to the end of the list of `routingKeys` for processing. For more information about message forwarding and routing, see [RFC 0094 Cross Domain Messaging](https://github.com/hyperledger/aries-rfcs/tree/main/concepts/0094-cross-domain-messaging).
 
 ### Adoption Messages
 
@@ -332,7 +332,7 @@ There is an optional courtesy error message stemming from an out-of-band message
 }
 
-See the [problem-report](https://github.com/hyperledger/aries-rfcs/tree/master/features/0035-report-problem) protocol for details on the items in the example.
+See the [problem-report](https://github.com/hyperledger/aries-rfcs/tree/main/features/0035-report-problem) protocol for details on the items in the example.
 
 ### Flow Overview
 
@@ -348,7 +348,9 @@ The handling of the response is specified by the protocol used.
 
 Using a standard out-of-band message encoding allows for easier interoperability between multiple projects and software platforms. Using a URL for that standard encoding provides a built in fallback flow for users who are unable to automatically process the message. Those new users will load the URL in a browser as a default behavior, and may be presented with instructions on how to install software capable of processing the message. Already onboarded users will be able to process the message without loading in a browser via mobile app URL capture, or via capability detection after being loaded in a browser.
 
-The standard out-of-band message format is a URL with a Base64URLEncoded json object as a query parameter.
+The standard out-of-band message format is a URL with a **Base64Url** encoded json object as a query parameter.
+
+Please note the difference between [Base64Url](https://datatracker.ietf.org/doc/html/rfc4648#section-5) and [Base64](https://datatracker.ietf.org/doc/html/rfc4648#section-4) encoding.
 
 The URL format is as follows, with some elements described below:
 
@@ -360,13 +362,13 @@ https://<domain>/<path>?oob=<outofbandMessage>
 
 > To do: We need to rationalize this approach `https://` approach with the use of a special protocol (e.g. `didcomm://`) that will enable handling of the URL on mobile devices to automatically invoke an installed app on both Android and iOS. A user must be able to process the out-of-band message on the device of the agent (e.g. when the mobile device can't scan the QR code because it is on a web page on device).
 
-The `<outofbandMessage>` is an agent plaintext message (not a DIDComm message) that has been base64 url encoded.
+The `<outofbandMessage>` is an agent plaintext message (not a DIDComm message) that has been Base64Url encoded such that the resulting string can be safely used in a URL.
 
 ```javascript
-outofband_message = b64urlencode(<outofbandMessage>)
+outofband_message = base64UrlEncode(<outofbandMessage>)
 
-During encoding, whitespace from the JSON string **SHOULD** be eliminated to keep the resulting out-of-band message string as short as possible.
+During Base64Url encoding, whitespace from the JSON string **SHOULD** be eliminated to keep the resulting out-of-band message string as short as possible.
 
 #### Example Out-of-Band Message Encoding
 
@@ -390,16 +392,16 @@ Whitespace removed:
 {"@type":"https://didcomm.org/out-of-band/1.0/invitation","@id":"69212a3a-d068-4f9d-a2dd-4741bca89af3","label":"Faber College","goal_code":"issue-vc","goal":"To issue a Faber College Graduate credential","handshake_protocols":["https://didcomm.org/didexchange/1.0","https://didcomm.org/connections/1.0"],"services":["did:sov:LjgpST2rjsoxYegQDRm7EL"]}

 
-Base 64 URL Encoded:
+Base64Url encoded:
 
 ```text
-eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCAiZ29hbF9jb2RlIjoiaXNzdWUtdmMiLCJnb2FsIjoiVG8gaXNzdWUgYSBGYWJlciBDb2xsZWdlIEdyYWR1YXRlIGNyZWRlbnRpYWwiLCJoYW5kc2hha2VfcHJvdG9jb2xzIjpbImh0dHBzOi8vZGlkY29tbS5vcmcvZGlkZXhjaGFuZ2UvMS4wIiwiaHR0cHM6Ly9kaWRjb21tLm9yZy9jb25uZWN0aW9ucy8xLjAiXSwic2VydmljZSI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0
+eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCJnb2FsX2NvZGUiOiJpc3N1ZS12YyIsImdvYWwiOiJUbyBpc3N1ZSBhIEZhYmVyIENvbGxlZ2UgR3JhZHVhdGUgY3JlZGVudGlhbCIsImhhbmRzaGFrZV9wcm90b2NvbHMiOlsiaHR0cHM6Ly9kaWRjb21tLm9yZy9kaWRleGNoYW5nZS8xLjAiLCJodHRwczovL2RpZGNvbW0ub3JnL2Nvbm5lY3Rpb25zLzEuMCJdLCJzZXJ2aWNlcyI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0=

 
-Example URL:
+Example URL with Base64Url encoded message:
 
 ```text
-http://example.com/ssi?oob=eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCAiZ29hbF9jb2RlIjoiaXNzdWUtdmMiLCJnb2FsIjoiVG8gaXNzdWUgYSBGYWJlciBDb2xsZWdlIEdyYWR1YXRlIGNyZWRlbnRpYWwiLCJoYW5kc2hha2VfcHJvdG9jb2xzIjpbImh0dHBzOi8vZGlkY29tbS5vcmcvZGlkZXhjaGFuZ2UvMS4wIiwiaHR0cHM6Ly9kaWRjb21tLm9yZy9jb25uZWN0aW9ucy8xLjAiXSwic2VydmljZSI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0
+http://example.com/ssi?oob=eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCJnb2FsX2NvZGUiOiJpc3N1ZS12YyIsImdvYWwiOiJUbyBpc3N1ZSBhIEZhYmVyIENvbGxlZ2UgR3JhZHVhdGUgY3JlZGVudGlhbCIsImhhbmRzaGFrZV9wcm90b2NvbHMiOlsiaHR0cHM6Ly9kaWRjb21tLm9yZy9kaWRleGNoYW5nZS8xLjAiLCJodHRwczovL2RpZGNvbW0ub3JnL2Nvbm5lY3Rpb25zLzEuMCJdLCJzZXJ2aWNlcyI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0=
 
 Out-of-band message URLs can be transferred via any method that can send text, including an email, SMS, posting on a website, or QR Code.
@@ -417,9 +419,9 @@ Subject: Your request to connect and receive your graduate verifiable credential
 
 Dear Alice,
 
-To receive your Faber College graduation certificate, click here to [connect](http://example.com/ssi?oob=eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCAiZ29hbF9jb2RlIjoiaXNzdWUtdmMiLCJnb2FsIjoiVG8gaXNzdWUgYSBGYWJlciBDb2xsZWdlIEdyYWR1YXRlIGNyZWRlbnRpYWwiLCJoYW5kc2hha2VfcHJvdG9jb2xzIjpbImh0dHBzOi8vZGlkY29tbS5vcmcvZGlkZXhjaGFuZ2UvMS4wIiwiaHR0cHM6Ly9kaWRjb21tLm9yZy9jb25uZWN0aW9ucy8xLjAiXSwic2VydmljZSI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0) with us, or paste the following into your browser:
+To receive your Faber College graduation certificate, click here to [connect](http://example.com/ssi?oob=eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCJnb2FsX2NvZGUiOiJpc3N1ZS12YyIsImdvYWwiOiJUbyBpc3N1ZSBhIEZhYmVyIENvbGxlZ2UgR3JhZHVhdGUgY3JlZGVudGlhbCIsImhhbmRzaGFrZV9wcm90b2NvbHMiOlsiaHR0cHM6Ly9kaWRjb21tLm9yZy9kaWRleGNoYW5nZS8xLjAiLCJodHRwczovL2RpZGNvbW0ub3JnL2Nvbm5lY3Rpb25zLzEuMCJdLCJzZXJ2aWNlcyI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0=) with us, or paste the following into your browser:
 
-http://example.com/ssi?oob=eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCAiZ29hbF9jb2RlIjoiaXNzdWUtdmMiLCJnb2FsIjoiVG8gaXNzdWUgYSBGYWJlciBDb2xsZWdlIEdyYWR1YXRlIGNyZWRlbnRpYWwiLCJoYW5kc2hha2VfcHJvdG9jb2xzIjpbImh0dHBzOi8vZGlkY29tbS5vcmcvZGlkZXhjaGFuZ2UvMS4wIiwiaHR0cHM6Ly9kaWRjb21tLm9yZy9jb25uZWN0aW9ucy8xLjAiXSwic2VydmljZSI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0
+http://example.com/ssi?oob=eyJAdHlwZSI6Imh0dHBzOi8vZGlkY29tbS5vcmcvb3V0LW9mLWJhbmQvMS4wL2ludml0YXRpb24iLCJAaWQiOiI2OTIxMmEzYS1kMDY4LTRmOWQtYTJkZC00NzQxYmNhODlhZjMiLCJsYWJlbCI6IkZhYmVyIENvbGxlZ2UiLCJnb2FsX2NvZGUiOiJpc3N1ZS12YyIsImdvYWwiOiJUbyBpc3N1ZSBhIEZhYmVyIENvbGxlZ2UgR3JhZHVhdGUgY3JlZGVudGlhbCIsImhhbmRzaGFrZV9wcm90b2NvbHMiOlsiaHR0cHM6Ly9kaWRjb21tLm9yZy9kaWRleGNoYW5nZS8xLjAiLCJodHRwczovL2RpZGNvbW0ub3JnL2Nvbm5lY3Rpb25zLzEuMCJdLCJzZXJ2aWNlcyI6WyJkaWQ6c292OkxqZ3BTVDJyanNveFllZ1FEUm03RUwiXX0=
 
 If you don't have an identity agent for holding credentials, you will be given instructions on how you can get one.
 
@@ -440,24 +442,33 @@ It seems inevitable that the length of some out-of-band message will be too long
   - `https://example.com/8E6nEcJ26TTE`
   - `https://example.com/sky/event/8DcnUW2h8m4jcfPdQ2uMN7/work-laptop-bag/s/u`
 - On receipt of this form of message, the agent **MUST** perform an HTTP GET to retrieve the associated out-of-band message. The agent **SHOULD** include an `Accept` header requesting the `application/json` MIME type.
-- The sender **MAY** include a `Content-Type` header specifying `application/json; charset=utf-8`. If so, the sender **MUST** return the invitation in JSON format.
-  - A sender may decide to wait to generate the full invitation until the redirection event of the shortened URL to the full length form dynamic, so that a single QR code can be used for distinct out-of-band messages.
-- The sender **MAY** respond with a `status_code` of `301` or `302` and a `Location` header specifying the long out-of-band message URL.
+- The sender **MAY** include a `Content-Type` header specifying `application/json; charset=utf-8`, and in the case where the agent included an `Accept` header for the `application/json` MIME type, the sender **MUST** include the header. If so, the sender **MUST** return the invitation in JSON format in the response body with a `status_code` of `200`.
+- The sender **MAY** respond with a `status_code` of `301` or `302` and include a `Location` header specifying the long out-of-band message URL.
   - This redirect option operates like many commercial URL shorteners. 
 - The sender **MUST** invalidate the URL after message retrieval or after an expiration time to prevent unintended parties from retrieving a copy of the message.
   - A sender **MUST NOT** use a commercial URL shortener unless it supports invalidating the URL.
 
 A usable QR code will always be able to be generated from the shortened form of the URL.
 
+
+#### URL Shortening Caveats
+
+Some HTTP libraries don't support stopping redirects from occuring on reception of a `301` or `302`, in this instance the redirect is automatically followed and will result in a response that **MAY** have a status of `200` and **MAY** contain a URL that can be processed as a normal `Out-of-Band` message.
+
+If the agent performs a HTTP GET with the `Accept` header requesting `application/json` MIME type the response can either contain the message in `json` or result in a redirect, processing of the response should attempt to determine which response type is received and process the message accordingly.
+
 #### Out-of-Band Message Publishing
 
 The _sender_ will publish or transmit the out-of-band message URL in a manner available to the intended _receiver_. After publishing, the sender is in the _await-response_ state, will the receiver is in the _prepare-response_ state.
 
 #### Out-of-Band Message Processing
 
-When they receiver receives the out-of-band message URL, there are two possible user flows, depending on whether the individual has an Aries agent. If the individual is new to Aries, they will likely load the URL in a browser. The resulting page **SHOULD** contain instructions on how to get started by installing an Aries agent. That install flow will transfer the out-of-band message to the newly installed software.
+If the receiver receives an `out-of-band` message in the form of a QR code, the receiver should attempt to decode the QR code to an out-of-band message URL for processing.
+
+When the receiver receives the out-of-band message URL, there are two possible user flows, depending on whether the individual has an Aries agent. If the individual is new to Aries, they will likely load the URL in a browser. The resulting page **SHOULD** contain instructions on how to get started by installing an Aries agent. That install flow will transfer the out-of-band message to the newly installed software.
+
+A user that already has those steps accomplished will have the URL received by software directly. That software will attempt to base64URL decode the string and can read the out-of-band message directly out of the `oob` query parameter, without loading the URL. If this process fails then the software should attempt the steps to [process a shortened URL](#url-shortening). 
 
-A user that already has those steps accomplished will have the URL received by software directly. That software will base64URL decode the string and can read the out-of-band message directly out of the `oob` query parameter, without loading the URL.
 
 > **NOTE**: In receiving the out-of-band message, the base64url decode implementation used **MUST**
 > correctly decode padded and unpadded base64URL encoded data.
@@ -524,7 +535,7 @@ If the receiver included a [`~service` decorator](../0056-service-decorator/READ
 ## Prior art
 
 - The out-of-band message/response process is similar to other key exchange protocols.
-- The [Connections](https://github.com/hyperledger/aries-rfcs/tree/master/features/0160-connection-protocol) and [DID Exchange](https://github.com/hyperledger/aries-rfcs/tree/master/features/0023-did-exchange) protocols have (or had) their own `invitation` method.
+- The [Connections](https://github.com/hyperledger/aries-rfcs/tree/main/features/0160-connection-protocol) and [DID Exchange](https://github.com/hyperledger/aries-rfcs/tree/main/features/0023-did-exchange) protocols have (or had) their own `invitation` method.
 - The `~service` decorator in combination with a request/response-type protocol message (such as present-proof/request) has previously used in place of the out-of-band `request` message.
 
 ## Unresolved questions


```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 21:29:11 +0000 UTC
    </div>
</div>

