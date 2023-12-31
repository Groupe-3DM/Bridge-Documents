# Retrieve details of a specific receiving record by ID

### URL

```text
api/v1/receivings/:id
```

### Method

```text
GET
```
### Parameters

| Name               | Type    | Required | Default | Description       |
|--------------------|---------|----------|---------|-------------------|

### Note

```text

```

### Auth required

```text
Yes
```

### Headers

```text
Content-Type: application/json
Accept: application/json
Authorization: Bearer ******************
```

### Request example

```json

```

### Success response


```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "id": 1,
    "client_id": 1,
    "client_name": "huyt",
    "carrier_id": 1,
    "carrier_name": "1",
    "warehouse_door_id": 1,
    "receiving_status_id": 7,
    "delivery_status_id": 1,
    "delivery_type_id": 1,
    "appointment_id": 1,
    "appointment_status_id": 1,
    "bill_lading": "45",
    "paperwork_provided": 1,
    "temperature_device_included": 1,
    "delivered_with_cod": 1,
    "single_pallet": 0,
    "multi_pallet": 0,
    "single_pallet_unloaded": 0,
    "multi_pallet_unloaded": 0,
    "carton_multi_pallet": 0,
    "carton_unloaded": 0,
    "pallet_provided": 0,
    "pallet_wrapped": 0,
    "pallet_reconfigured": 0,
    "tth": 0,
    "cartons": 0,
    "pallets": 0,
    "total_received_unit": 0,
    "tracking": null,
    "comments": null,
    "file": null,
    "duty_tax_paid": null,
    "container_size": null,
    "seal_number": "hh",
    "container_number": "hh",
    "asn": null,
    "scheduled_date": "2023-01-23",
    "scheduled_time": "11:00:00",
    "received_date": "2023-01-23",
    "received_time": "08:00:00",
    "received_by": "kl",
    "approved_date": "2023-01-23",
    "approved_time": null,
    "approved_by": "Genming Zhao",
    "purchase_order_number": "99999999999",
    "total_expected_unit": "222",
    "pallet_unloaded": 0,
    "delivery_detail_id": null,
    "cartons_delivered": 0,
    "pallets_delivered": 0,
    "receiving_items": [
      {
        "id": 84,
        "receiving_id": 1,
        "item_id": 1,
        "sku": null,
        "lot": null,
        "expiry_date": null,
        "uom_type_id": 1,
        "uom_quantity": 1,
        "expected_quantity": null,
        "received_quantity": null,
        "location_id": null,
        "weight": "0.00",
        "count_method": null,
        "receiving_item_status_id": null,
        "receiving_item_reason_id": null,
        "receiving_po_id": 1,
        "quantity": 0,
        "item_index": null,
        "sent_to_proxpert_on": null,
        "status": 1,
        "created_by": null,
        "created_at": "2023-11-05T14:28:47.000000Z",
        "finalized_by": null,
        "finalized_at": null,
        "warehouse_id": null,
        "client_id": null,
        "is_damaged": 0,
        "other_damaged_reason": null,
        "receiving_item_condition_id": null,
        "location_name": null
      },
      {
        "id": 85,
        "receiving_id": 1,
        "item_id": 2,
        "sku": null,
        "lot": null,
        "expiry_date": null,
        "uom_type_id": 1,
        "uom_quantity": 1,
        "expected_quantity": null,
        "received_quantity": null,
        "location_id": null,
        "weight": "0.00",
        "count_method": null,
        "receiving_item_status_id": null,
        "receiving_item_reason_id": null,
        "receiving_po_id": 1,
        "quantity": 0,
        "item_index": null,
        "sent_to_proxpert_on": null,
        "status": 1,
        "created_by": null,
        "created_at": "2023-11-05T14:28:47.000000Z",
        "finalized_by": null,
        "finalized_at": null,
        "warehouse_id": null,
        "client_id": null,
        "is_damaged": 0,
        "other_damaged_reason": null,
        "receiving_item_condition_id": null,
        "location_name": null
      },
      {
        "id": 86,
        "receiving_id": 1,
        "item_id": 3,
        "sku": null,
        "lot": null,
        "expiry_date": null,
        "uom_type_id": 1,
        "uom_quantity": 1,
        "expected_quantity": null,
        "received_quantity": null,
        "location_id": null,
        "weight": "0.00",
        "count_method": null,
        "receiving_item_status_id": null,
        "receiving_item_reason_id": null,
        "receiving_po_id": 1,
        "quantity": 0,
        "item_index": null,
        "sent_to_proxpert_on": null,
        "status": 1,
        "created_by": null,
        "created_at": "2023-11-06T00:30:44.000000Z",
        "finalized_by": null,
        "finalized_at": null,
        "warehouse_id": null,
        "client_id": null,
        "is_damaged": 0,
        "other_damaged_reason": null,
        "receiving_item_condition_id": null,
        "location_name": null
      },
      {
        "id": 87,
        "receiving_id": 1,
        "item_id": 4,
        "sku": null,
        "lot": null,
        "expiry_date": null,
        "uom_type_id": 1,
        "uom_quantity": 1,
        "expected_quantity": null,
        "received_quantity": null,
        "location_id": null,
        "weight": "0.00",
        "count_method": null,
        "receiving_item_status_id": null,
        "receiving_item_reason_id": null,
        "receiving_po_id": 1,
        "quantity": 0,
        "item_index": null,
        "sent_to_proxpert_on": null,
        "status": 1,
        "created_by": null,
        "created_at": "2023-11-06T00:31:29.000000Z",
        "finalized_by": null,
        "finalized_at": null,
        "warehouse_id": null,
        "client_id": null,
        "is_damaged": 0,
        "other_damaged_reason": null,
        "receiving_item_condition_id": null,
        "location_name": null
      }
    ]
  }
}
```