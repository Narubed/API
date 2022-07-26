# compensation 
## ค่าตอบแทนการส่งงาน NBA Platform

## https://api.nbadigitalservice.com/v1/office

### การดึงข้อมูลของ compensation ทั้งหมด

```http
GET /compensation
```

### การดึงข้อมูลของ compensation ผ่านไอดี

```http
GET /compensation/:_id
_id=62860054821f7b69619f254
```

### การเพิ่มข้อมูล compensation

```http
POST /compensation
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `com_member_id` | `string` | **id ผู้ใช้** |
| `com_project_id` | `string` | **id โปรเจค** |
| `com_product_price` | `number` | **ราคาสินค้า** |
| `com_freight` | `number` | **ค่าขนส่ง** |
| `com_vat` | `number` | **ภาษี 7 เปอร์** |
| `com_cost_price` | `number` | **ราคาทุน** |
| `com_cost_profit` | `number` | **กำไรสุทธูิ** |
| `com_lv_owner` | `number` | **เปอร์เซ็นคนส่งงาน** |
| `com_lv_one` | `number` | **เปอร์เซ็นชั้น1** |
| `com_lv_two` | `number` | **เปอร์เซ็นชั่น2** |
| `com_lv_tree` | `number` | **เปอร์เซ็นชั้น3** |
| `com_lv_office` | `number` | **เปอร์เซ็น สนง.ใหญ่** |
| `com_all_sela` | `number` | **all sela** |
| `com_funds` | `number` | **เงินกองทุน** |
| `com_province` | `number` | **เปอร์เซ็นจังหวัด** |
| `com_district` | `number` | **เปอร์เซ็นอำเภอ** |
| `com_sub_district` | `number` | **เปอร์เซ็นตำบล** |
| `com_bonus_staff` | `number` | **โบนัสพนักงาน** |
| `com_timestamp` | `date` | **วันเวลาที่เพิ่มข้อมูล** | **default: new Date()** |

### การแก้ไขข้อมูล compensation

```http
PUT /compensation/:_id
_id=62860054821f7b69619f254
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `com_member_id` | `string` | **id ผู้ใช้** |
| `com_project_id` | `string` | **id โปรเจค** |
| `com_product_price` | `number` | **ราคาสินค้า** |
| `com_freight` | `number` | **ค่าขนส่ง** |
| `com_vat` | `number` | **ภาษี 7 เปอร์** |
| `com_cost_price` | `number` | **ราคาทุน** |
| `com_cost_profit` | `number` | **กำไรสุทธูิ** |
| `com_lv_owner` | `number` | **เปอร์เซ็นคนส่งงาน** |
| `com_lv_one` | `number` | **เปอร์เซ็นชั้น1** |
| `com_lv_two` | `number` | **เปอร์เซ็นชั่น2** |
| `com_lv_tree` | `number` | **เปอร์เซ็นชั้น3** |
| `com_lv_office` | `number` | **เปอร์เซ็น สนง.ใหญ่** |
| `com_all_sela` | `number` | **all sela** |
| `com_funds` | `number` | **เงินกองทุน** |
| `com_province` | `number` | **เปอร์เซ็นจังหวัด** |
| `com_district` | `number` | **เปอร์เซ็นอำเภอ** |
| `com_sub_district` | `number` | **เปอร์เซ็นตำบล** |
| `com_bonus_staff` | `number` | **โบนัสพนักงาน** |
| `com_timestamp` | `date` | **วันเวลาที่เพิ่มข้อมูล** | **default: new Date()** |

### การลบข้อมูล compensation

```http
DELETE /compensation/:_id
_id=62860054821f7b69619f254
```

### การดึงข้อมูล compensation ด้วยไอดีผู้ใช่

```http
GET /compensation/member/:_id
_id=62860054821f7b69619f254
```
