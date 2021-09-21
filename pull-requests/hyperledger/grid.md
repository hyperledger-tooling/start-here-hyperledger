---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/941" class=".btn">#941</a>
            </td>
            <td>
                <b>
                    Fix Client `ROLES_ENDPOINT` const
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the `ROLES_ENDPOINT` const, defined for the
`ReqwestPikeClient`, to `ROLE_ENDPOINT` and updates the value from
"roles" to "role". The role endpoint is singular.

Signed-off-by: Shannyn Telander <telander@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 21:54:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/939" class=".btn">#939</a>
            </td>
            <td>
                <b>
                    Hookup PO SDE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This sets up the state delta export for purchase order events. This PR also adds the conversion methods to `EventError` for the purchase order store errors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 18:40:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/936" class=".btn">#936</a>
            </td>
            <td>
                <b>
                    Update PO version protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the PO version proto to reflect that a version can have multiple revisions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 18:34:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/935" class=".btn">#935</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Disable Jenkins CI builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                GitHub Actions will be used going forward instead.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 14:10:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/934" class=".btn">#934</a>
            </td>
            <td>
                <b>
                    Disable Jenkins CI builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                GitHub Actions will be used going forward instead.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 13:58:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/933" class=".btn">#933</a>
            </td>
            <td>
                <b>
                    Implement data validation module and PO validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements a new data validation module. It includes new functionality to validate purchase orders with the GS1 Order XML 3.4 specification. The GDSN validation functionality was also moved here.

To test:

- navigate to CLI and `$ cargo build --features=experimental`
- Navigate to root grid directory
- `$ export PATH=$PATH:$(pwd)/target/debug`
- Copy the following xml into a file called `test-po.xml`:
```
<?xml version="1.0" encoding="UTF-8"?>
<order:orderMessage xmlns:order="urn:gs1:ecom:order:xsd:3"
    xmlns:sh="http://www.unece.org/cefact/namespaces/StandardBusinessDocumentHeader"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:gs1:ecom:order:xsd:3 ../Schemas/gs1/ecom/Order.xsd">
    <sh:StandardBusinessDocumentHeader>
        <sh:HeaderVersion>1.0</sh:HeaderVersion>
        <sh:Sender>
            <sh:Identifier Authority="GS1"/>
            <sh:ContactInformation>
                <sh:Contact>John Doe</sh:Contact>
                <sh:EmailAddress>John_Doe@purchasing.XYZretailer.com</sh:EmailAddress>
                <sh:TelephoneNumber>+1-212-555-2122</sh:TelephoneNumber>
                <sh:ContactTypeIdentifier>Buyer</sh:ContactTypeIdentifier>
            </sh:ContactInformation>
        </sh:Sender>
        <sh:Receiver>
            <sh:Identifier Authority="GS1"/>
            <sh:ContactInformation>
                <sh:Contact>Mary Smith</sh:Contact>
                <sh:EmailAddress>Mary_Smith@widgets.com</sh:EmailAddress>
                <sh:TelephoneNumber>+1-312-555-2125</sh:TelephoneNumber>
                <sh:ContactTypeIdentifier>Seller</sh:ContactTypeIdentifier>
            </sh:ContactInformation>
        </sh:Receiver>
        <sh:DocumentIdentification>
            <sh:Standard>GS1</sh:Standard>
            <sh:TypeVersion>3.4</sh:TypeVersion>
            <sh:InstanceIdentifier>100002</sh:InstanceIdentifier>
            <sh:Type/>
            <sh:MultipleType>false</sh:MultipleType>
            <sh:CreationDateAndTime>asdf</sh:CreationDateAndTime>
        </sh:DocumentIdentification>
    </sh:StandardBusinessDocumentHeader>
    <order>
        <creationDateTime>2021-07-14T12:00:00.000-01:00</creationDateTime>
        <documentStatusCode>ORIGINAL</documentStatusCode>
        <orderIdentification>
            <entityIdentification>PO3352</entityIdentification>
            <contentOwner>
                <gln>5412345000013</gln>
            </contentOwner>
        </orderIdentification>
        <buyer>
            <gln>5412345000013</gln>
        </buyer>
        <seller>
            <gln>4098765000010</gln>
        </seller>
        <orderLogisticalInformation>
            <shipFrom>
                <gln>4098765000010</gln>
            </shipFrom>
            <shipTo>
                <gln>5412345000037</gln>
            </shipTo>
            <inventoryLocation>
                <gln>4098765000010</gln>
            </inventoryLocation>
            <orderLogisticalDateInformation>
                <requestedDeliveryDateTime>
                    <date>2011-03-11</date>
                    <time>12:00:00.000-01:00</time>
                </requestedDeliveryDateTime>
                <requestedShipDateTime>
                    <date>2011-03-11</date>
                    <time>12:00:00.000-01:00</time>
                </requestedShipDateTime>
            </orderLogisticalDateInformation>
        </orderLogisticalInformation>
        <orderLineItem>
            <lineItemNumber>1</lineItemNumber>
            <requestedQuantity measurementUnitCode="EA">10</requestedQuantity>
            <netAmount currencyCode="EUR">100.00</netAmount>
            <netPrice currencyCode="EUR">10.00</netPrice>
            <transactionalTradeItem>
                <gtin>40987650000345</gtin>
            </transactionalTradeItem>
        </orderLineItem>
        <orderLineItem>
            <lineItemNumber>2</lineItemNumber>
            <requestedQuantity measurementUnitCode="EA">24</requestedQuantity>
            <netAmount currencyCode="EUR">4659</netAmount>
            <netPrice currencyCode="EUR">194.125</netPrice>
            <transactionalTradeItem>
                <gtin>40987650000346</gtin>
            </transactionalTradeItem>
        </orderLineItem>
    </order>
</order:orderMessage>
```
- `$ grid po version create test-po --org myorg --order-xml test-po.xml`
The PO name and org aren't used since we arent actually creating anything. You should see a log message: "Purchase order is valid"
- Try changing some values in the PO XML to make it invalid. After running the validation command you should see the validation errors and a dump of the XML.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 20:10:37 +0000 UTC
    </div>
</div>

