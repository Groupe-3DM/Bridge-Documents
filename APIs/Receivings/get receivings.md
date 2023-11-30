# Retrieve a list of receiving(s) with query builder.



`endpoint: api/v1/items`

`method: GET`

**searchable query fields**

| Name                | Type                                          |
|---------------------|-----------------------------------------------|
| client_id           | number/array                                  |
| asn                 | string                                        |
| receiving_status_id | integer                                       |
| arrival_date        | date                                          |
| arrival_time        | time                                          |
| sku                 | string                                        |
| appointment_id      | string                                        |
| sort_by             | any of above field                            |
| sort_order          | DESC/ASC                                      |
| limit               | number(<200)                                  |
| list                | count/take/auto-complete (default: paginated) |


* `query's example: asn=xxxx&receiving_status_id=1&limit=20&list=all`
* 
### Response

```json
{
  "success": true,
  "message": "Operation has been successfully completed!",
  "data": {
    "data": [
      {
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
        "sent_to_proxpert_on": null,
        "approved_by": "Genming Zhao",
        "purchase_order_number": "99999999999",
        "total_expected_unit": "222",
        "pallet_unloaded": 0,
        "delivery_detail_id": null,
        "cartons_delivered": 0,
        "pallets_delivered": 0
      }
    ],
    "current_page": 1,
    "last_page": 1,
    "from": 1,
    "to": 1,
    "total": 1,
    "per_page": 1
  }
}
```