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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/932" class=".btn">#932</a>
            </td>
            <td>
                <b>
                    Update PO store for updated protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the PO store to account for the changes to the PO protobuf messages. This updates the schemas, DB models, Grid structs, DB operations, and REST API to account for the different fields in the updated messages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 19:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/931" class=".btn">#931</a>
            </td>
            <td>
                <b>
                    Added the libzmq3-dev dependency for building in Debian(Ubuntu)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi, I have added the needed pre-requisite for building Grid on Debian(Ubuntu).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 12:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/929" class=".btn">#929</a>
            </td>
            <td>
                <b>
                    BACKPORT 0-2: Add GHA files
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
        Created At 2021-09-09 20:18:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/928" class=".btn">#928</a>
            </td>
            <td>
                <b>
                    Add state methods to get/set purchase order versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds implementations for `get_purchase_order_version` and `set_purchase_order_version` for `PurchaseOrderState`. This also adds tests for all of the state methods (including the newly implemented ones).  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 20:00:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/927" class=".btn">#927</a>
            </td>
            <td>
                <b>
                    Add `list_purchase_order_versions` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a `list_purchase_order_versions` operation to the purchase
order store. This operation gets a list of purchase order versions for a
gived purchase order. This also includes that version's revisions.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 16:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/925" class=".btn">#925</a>
            </td>
            <td>
                <b>
                    Add `buyer` and `seller` org fields to Purchase Order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the `PurchaseOrderPayload` to remove the `org_id` field, as the organizations are now being recorded in the purchase order itself. This also updates the `CreatePurchaseOrderPayload` and `PurchaseOrder` struct in state to support a `buyer_org` and `seller_org` fields for the purchase order. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 15:28:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/924" class=".btn">#924</a>
            </td>
            <td>
                <b>
                    Add `get_purchase_order_version` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a `get_purchase_order_version` operation. This fetches a PO
version and its associated revisions and returns the Grid representation
of them.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 21:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/923" class=".btn">#923</a>
            </td>
            <td>
                <b>
                    Update `add_purchase_order` operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the `add_purchase_order` operation to properly add/update POs, versions, and revisions while avoiding unnecessary db updates.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 20:23:43 +0000 UTC
    </div>
</div>

