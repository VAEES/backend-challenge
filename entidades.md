[Voltar](./README.md)

## Entidades

| Products |
|---|

| Column | DataType(size) |
|---|:---:|
|id|PRIMARY KEY INTEGER AUTO INCREMENT OR UUID|
|title|VARCHAR(30)|
|price|DECIMAL(11,2)|
|description|VARCHAR(100)|
|category|VARCHAR(50)|
|image|VARCHAR(200)|
---
| Users |
|---|

| Column | DataType(size) |
|---|:---:|
|id|PRIMARY KEY INTEGER AUTO INCREMENT OR UUID|
|email|VARCHAR(100)|
|username|VARCHAR(50)|
|password|VARCHAR(50)|
|first_name|VARCHAR(50)|
|last_name|VARCHAR(50)|
---
| Purchase Orders |
|---|

| Column | DataType(size) |
|---|:---:|
|id|PRIMARY KEY INTEGER AUTO INCREMENT OR UUID|
|user_id|FK users|
|date|DateTime|
---
| Purchase Order Items |
|---|

| Column | DataType(size) |
|---|:---:|
|product_id|FK products|
|purchase_order_id|FK purchase_orders|
|quantity|Integer|
|price|Decimal(15,2)|
