# Login to retrieve authenticated user's information

### URL

```text
api/v1/login
```

### Method

```text
POST
```

### Parameters


| Name     | Type   | Required | Default | Description |
|----------|--------|----------|---------|-------------|
| email    | email  | Y        |         |             |
| password | string | Y        |         |             |

### Auth required
```text
NO
```


### Headers
```text
Content-Type: application/json
Accept: application/json

```



### Request example

```json
{
  "email": "your-email@domain.com",
  "password": "xxxxxxx"
}
```

### Success example

```json
{
  "success": true,
  "data": {
    "token": "xxxxxxxxx",
    "name": "Your name",
    "user": {
      "id": 2,
      "salutation_id": 4,
      "first_name": "Your first name",
      "last_name": "Last name",
      "email": "xxxx@email.com",
      "home_phone": "514-123-1234",
      "cell_phone": "514-123-1234",
      "office_phone": "514-123-1234",
      "office_extension": "514-123-1234",
      "notifying": 1,
      "address1": "514-123-1234",
      "address2": null,
      "postal_code": "h9r5x7",
      "city": "montreal",
      "province_id": 612,
      "country_id": 38,
      "language_id": 1,
      "warehouse_id": 11,
      "status": 1,
      "department_id": 1,
      "employee": 1,
      "job_title": developer",
      "image": "male.png",
      "notes": "test",
      "dashboard": 0,
      "scanner_gun": 0,
      "prox": 0,
      "portal": 0,
      "email_verified_at": "2022-09-28 11:45:20",
      "creator_id": null,
      "synch_message": null,
      "synch_status": null,
      "production_user": 0,
      "order_error": 1,
      "item_error": 1,
      "permissions": [
        {
          "id": 170,
          "name": "menu-permissions",
          "internal": 1,
          "external": 0,
          "parent_id": 171
        },
        {
          "id": 171,
          "name": "menu-security",
          "internal": 1,
          "external": 1,
          "parent_id": 177
        },
        {
          "id": 172,
          "name": "menu-dashboard",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 173,
          "name": "menu-roles",
          "internal": 1,
          "external": 0,
          "parent_id": 171
        },
        {
          "id": 174,
          "name": "permissions-create",
          "internal": 1,
          "external": 0,
          "parent_id": 170
        },
        {
          "id": 175,
          "name": "permissions-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 170
        },
        {
          "id": 176,
          "name": "permissions-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 170
        },
        {
          "id": 177,
          "name": "menu-admin",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 178,
          "name": "menu-appointment",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 179,
          "name": "menu-billing",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 180,
          "name": "menu-billing_bill",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 181,
          "name": "menu-billing_details",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 182,
          "name": "menu-billing_categories",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 183,
          "name": "menu-billing_client_pricing",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 184,
          "name": "menu-billing_unit_of_measure",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 185,
          "name": "menu-billing_line_charges",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 186,
          "name": "menu-taxes",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 187,
          "name": "menu-tax_rates",
          "internal": 1,
          "external": 0,
          "parent_id": 186
        },
        {
          "id": 188,
          "name": "menu-tax_classes",
          "internal": 1,
          "external": 0,
          "parent_id": 186
        },
        {
          "id": 189,
          "name": "menu-return",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 190,
          "name": "menu-pickings",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 191,
          "name": "menu-replenishment",
          "internal": 1,
          "external": 0,
          "parent_id": 222
        },
        {
          "id": 192,
          "name": "menu-packing",
          "internal": 1,
          "external": 0,
          "parent_id": 222
        },
        {
          "id": 193,
          "name": "menu-shipping",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 194,
          "name": "menu-orders",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 195,
          "name": "menu-receiving",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 196,
          "name": "menu-receiving_mobile",
          "internal": 1,
          "external": 0,
          "parent_id": 222
        },
        {
          "id": 197,
          "name": "menu-purchase_order",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 198,
          "name": "menu-jobs",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 199,
          "name": "menu-inventory",
          "internal": 1,
          "external": 1,
          "parent_id": 221
        },
        {
          "id": 200,
          "name": "menu-transactions",
          "internal": 1,
          "external": 0,
          "parent_id": 221
        },
        {
          "id": 201,
          "name": "menu-quick_zone",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 202,
          "name": "menu-item",
          "internal": 1,
          "external": 1,
          "parent_id": 221
        },
        {
          "id": 203,
          "name": "menu-barcode_generator",
          "internal": 1,
          "external": 1,
          "parent_id": 221
        },
        {
          "id": 204,
          "name": "menu-clients",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 205,
          "name": "menu-client",
          "internal": 1,
          "external": 1,
          "parent_id": 204
        },
        {
          "id": 206,
          "name": "menu-supplier",
          "internal": 1,
          "external": 1,
          "parent_id": 204
        },
        {
          "id": 207,
          "name": "menu-supply",
          "internal": 1,
          "external": 0,
          "parent_id": 204
        },
        {
          "id": 208,
          "name": "menu-warehouse",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 209,
          "name": "menu-location",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 210,
          "name": "menu-user",
          "internal": 1,
          "external": 1,
          "parent_id": 171
        },
        {
          "id": 211,
          "name": "menu-system",
          "internal": 1,
          "external": 0,
          "parent_id": 177
        },
        {
          "id": 212,
          "name": "menu-platforms",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 213,
          "name": "menu-country",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 214,
          "name": "menu-languages",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 215,
          "name": "menu-holiday",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 216,
          "name": "menu-departments",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 217,
          "name": "menu-province",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 218,
          "name": "menu-carrier",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 219,
          "name": "menu-settings",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 220,
          "name": "menu-profile",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 221,
          "name": "menu-products",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 222,
          "name": "menu-operational_functions",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 223,
          "name": "menu-mobile_layout",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 224,
          "name": "menu-mobile_inventory",
          "internal": 1,
          "external": 0,
          "parent_id": 223
        },
        {
          "id": 225,
          "name": "menu-mobile_items",
          "internal": 1,
          "external": 0,
          "parent_id": 223
        },
        {
          "id": 226,
          "name": "menu-mobile_picking",
          "internal": 1,
          "external": 0,
          "parent_id": 223
        },
        {
          "id": 227,
          "name": "menu-mobile_receiving",
          "internal": 1,
          "external": 0,
          "parent_id": 223
        },
        {
          "id": 228,
          "name": "menu-mobile_replenishment",
          "internal": 1,
          "external": 0,
          "parent_id": 223
        },
        {
          "id": 229,
          "name": "menu-logs",
          "internal": 1,
          "external": 0,
          "parent_id": null
        },
        {
          "id": 232,
          "name": "roles-create",
          "internal": 1,
          "external": 0,
          "parent_id": 173
        },
        {
          "id": 233,
          "name": "roles-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 173
        },
        {
          "id": 234,
          "name": "roles-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 173
        },
        {
          "id": 274,
          "name": "logs-view",
          "internal": 1,
          "external": 0,
          "parent_id": 229
        },
        {
          "id": 275,
          "name": "appointment-create",
          "internal": 1,
          "external": 0,
          "parent_id": 178
        },
        {
          "id": 276,
          "name": "billing-create",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 277,
          "name": "billing-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 278,
          "name": "billing-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 179
        },
        {
          "id": 279,
          "name": "client-create",
          "internal": 1,
          "external": 0,
          "parent_id": 205
        },
        {
          "id": 280,
          "name": "client-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 205
        },
        {
          "id": 281,
          "name": "client-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 205
        },
        {
          "id": 282,
          "name": "inventory-transfer_to_location",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 283,
          "name": "inventory-transfer_sku_to_sku",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 285,
          "name": "inventory-transfer_whs_to_whs",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 287,
          "name": "item-create",
          "internal": 1,
          "external": 0,
          "parent_id": 202
        },
        {
          "id": 288,
          "name": "item-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 202
        },
        {
          "id": 289,
          "name": "item-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 202
        },
        {
          "id": 290,
          "name": "location-create",
          "internal": 1,
          "external": 0,
          "parent_id": 209
        },
        {
          "id": 291,
          "name": "location-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 209
        },
        {
          "id": 292,
          "name": "location-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 209
        },
        {
          "id": 293,
          "name": "orders-change_order_status",
          "internal": 1,
          "external": 0,
          "parent_id": 194
        },
        {
          "id": 294,
          "name": "orders-edit",
          "internal": 1,
          "external": 1,
          "parent_id": 194
        },
        {
          "id": 295,
          "name": "purchase_order-create",
          "internal": 1,
          "external": 1,
          "parent_id": 197
        },
        {
          "id": 296,
          "name": "purchase_order-edit",
          "internal": 1,
          "external": 1,
          "parent_id": 197
        },
        {
          "id": 297,
          "name": "purchase_order-view_price",
          "internal": 1,
          "external": 0,
          "parent_id": 197
        },
        {
          "id": 298,
          "name": "quick_zone-create",
          "internal": 1,
          "external": 0,
          "parent_id": 201
        },
        {
          "id": 299,
          "name": "quick_zone-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 201
        },
        {
          "id": 300,
          "name": "quick_zone-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 201
        },
        {
          "id": 301,
          "name": "quick_zone-replenishment",
          "internal": 1,
          "external": 0,
          "parent_id": 201
        },
        {
          "id": 302,
          "name": "return-create",
          "internal": 1,
          "external": 0,
          "parent_id": 189
        },
        {
          "id": 303,
          "name": "return-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 189
        },
        {
          "id": 304,
          "name": "return-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 189
        },
        {
          "id": 305,
          "name": "return-change_status",
          "internal": 1,
          "external": 0,
          "parent_id": 189
        },
        {
          "id": 306,
          "name": "user-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 210
        },
        {
          "id": 307,
          "name": "user-create",
          "internal": 1,
          "external": 0,
          "parent_id": 210
        },
        {
          "id": 308,
          "name": "system-create",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 309,
          "name": "system-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 310,
          "name": "system-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        },
        {
          "id": 311,
          "name": "warehouse-create",
          "internal": 1,
          "external": 0,
          "parent_id": 208
        },
        {
          "id": 312,
          "name": "warehouse-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 208
        },
        {
          "id": 313,
          "name": "inventory-create",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 314,
          "name": "orders-create",
          "internal": 1,
          "external": 1,
          "parent_id": 194
        },
        {
          "id": 315,
          "name": "orders-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 194
        },
        {
          "id": 316,
          "name": "user-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 210
        },
        {
          "id": 317,
          "name": "warehouse-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 208
        },
        {
          "id": 319,
          "name": "appointment-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 178
        },
        {
          "id": 320,
          "name": "appointment-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 178
        },
        {
          "id": 321,
          "name": "purchase_order-change_status",
          "internal": 1,
          "external": 0,
          "parent_id": 197
        },
        {
          "id": 322,
          "name": "appointment-cancel",
          "internal": 1,
          "external": 0,
          "parent_id": 178
        },
        {
          "id": 324,
          "name": "item-edit_sku",
          "internal": 1,
          "external": 0,
          "parent_id": 202
        },
        {
          "id": 325,
          "name": "item-resend_to_proxpert",
          "internal": 1,
          "external": 0,
          "parent_id": 202
        },
        {
          "id": 326,
          "name": "item-kitting",
          "internal": 1,
          "external": 0,
          "parent_id": 202
        },
        {
          "id": 327,
          "name": "return-view",
          "internal": 1,
          "external": 1,
          "parent_id": 189
        },
        {
          "id": 329,
          "name": "receiving-edit",
          "internal": 1,
          "external": 0,
          "parent_id": 195
        },
        {
          "id": 330,
          "name": "receiving-create",
          "internal": 1,
          "external": 0,
          "parent_id": 195
        },
        {
          "id": 331,
          "name": "receiving-delete",
          "internal": 1,
          "external": 0,
          "parent_id": 195
        },
        {
          "id": 332,
          "name": "receiving-print_tags",
          "internal": 1,
          "external": 0,
          "parent_id": 195
        },
        {
          "id": 333,
          "name": "orders-batch",
          "internal": 1,
          "external": 0,
          "parent_id": 194
        },
        {
          "id": 334,
          "name": "location-print",
          "internal": 1,
          "external": 0,
          "parent_id": 209
        },
        {
          "id": 335,
          "name": "item-print",
          "internal": 1,
          "external": 0,
          "parent_id": 202
        },
        {
          "id": 337,
          "name": "inventory-location_transfer",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 338,
          "name": "inventory-hold",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 339,
          "name": "inventory-adjust",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 340,
          "name": "inventory-transfer",
          "internal": 1,
          "external": 0,
          "parent_id": 199
        },
        {
          "id": 342,
          "name": "orders-cancel",
          "internal": 1,
          "external": 1,
          "parent_id": 194
        },
        {
          "id": 343,
          "name": "orders-release",
          "internal": 1,
          "external": 0,
          "parent_id": 194
        },
        {
          "id": 344,
          "name": "orders-import",
          "internal": 1,
          "external": 1,
          "parent_id": 194
        },
        {
          "id": 345,
          "name": "item-view",
          "internal": 1,
          "external": 1,
          "parent_id": 202
        },
        {
          "id": 346,
          "name": "orders-view",
          "internal": 1,
          "external": 1,
          "parent_id": 194
        },
        {
          "id": 347,
          "name": "receiving-finalized",
          "internal": 1,
          "external": 0,
          "parent_id": 195
        },
        {
          "id": 348,
          "name": "orders-integration",
          "internal": 1,
          "external": 0,
          "parent_id": 194
        },
        {
          "id": 349,
          "name": "receiving-details",
          "internal": 1,
          "external": 1,
          "parent_id": 195
        },
        {
          "id": 350,
          "name": "menu-serial_number",
          "internal": 1,
          "external": 0,
          "parent_id": 222
        },
        {
          "id": 351,
          "name": "menu-support",
          "internal": 1,
          "external": 1,
          "parent_id": null
        },
        {
          "id": 352,
          "name": "orders-quick_batch",
          "internal": 1,
          "external": 0,
          "parent_id": 194
        },
        {
          "id": 353,
          "name": "menu-errors",
          "internal": 1,
          "external": 0,
          "parent_id": 211
        }
      ],
      "clients": [
        6046,
        6083,
        6084,
        9999
      ],
      "roles": [
        1
      ]
    }
  },
  "message": "Operation has been successfully completed!"
}
```