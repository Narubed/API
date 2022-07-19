# art_work

## https://api.nbadigitalservice.com/v1/platform/project/artwork

### การดึงข้อมูลของ art_work ทั้งหมด

```http
GET /
```

### การดึงข้อมูลของ art_work ผ่านไอดี

```http
GET /:_id
_id=62860054821f7b69619f254
```

### การเพิ่มข้อมูล art_work

```http
POST /
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `cus_name` | `string` | **ชื่อลูกค้า** |
| `cus_tel` | `string` | **เบอร์โทร** |
| `cus_lineid` | `string` | **ไอดีไลน์** | **default: " "** |
| `cus_address` | `string` | **ที่อยุ่จัดส่ง กรณีมีที่อยู่จัดส่ง** | **default:ไม่มีการจัดส่ง** |
| `project_type` | `string` | **ประเภทของโปรเจค เช่น vinyl, rubber_stamp เป็นต้น** |
| `project_detail` | `array` | **รายละเอียดเกี่ยวกับโปรเจค แต่ละอย่างเก็บไม่เหมือนกัน** |
| `project_sentprice` | `number` | **ราคาจัดส่ง กรณีมีการจัดส่ง** | **default: 0** |
| `project_total` | `number` | **ราคารวมโปรเจคนี้** | **default: 0** |
| `project_cost` | `number` | **ต้นทุนสำหรับโปรเจคนี้** | **default: 0** |
| `vat` | `number` | **ภาษี 7 เปอร์เซ็น** | **default: 0** |
| `project_status` | `string` | **สถานะโปรเจค** | **default: paycheck** |
| `img_slip` | `file` | **รูปหลักฐานการชำระเงิน โฟรเดอร์สลิปแจ้งชำระเงินโปรเจค** |
| `tracking_number` | `string` | **เลขติดตามพัสดุกรณีมีการจัดส่ง** | **default: ""** |
| `express_brand` | `string` | **แบรนด์ขนส่ง** | **default: ""** |
| `timestamp` | `date` | **วันเวลาที่เริ่มโปรเจค** | **default: 0** |

### การแก้ไขข้อมูล art_work

```http
PUT /:_id
_id=62860054821f7b69619f254
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `cus_name` | `string` | **ชื่อลูกค้า** |
| `cus_tel` | `string` | **เบอร์โทร** |
| `cus_lineid` | `string` | **ไอดีไลน์** | **default: " "** |
| `cus_address` | `string` | **ที่อยุ่จัดส่ง กรณีมีที่อยู่จัดส่ง** | **default:ไม่มีการจัดส่ง** |
| `project_type` | `string` | **ประเภทของโปรเจค เช่น vinyl, rubber_stamp เป็นต้น** |
| `project_detail` | `array` | **รายละเอียดเกี่ยวกับโปรเจค แต่ละอย่างเก็บไม่เหมือนกัน** |
| `project_sentprice` | `number` | **ราคาจัดส่ง กรณีมีการจัดส่ง** | **default: 0** |
| `project_total` | `number` | **ราคารวมโปรเจคนี้** | **default: 0** |
| `project_cost` | `number` | **ต้นทุนสำหรับโปรเจคนี้** | **default: 0** |
| `vat` | `number` | **ภาษี 7 เปอร์เซ็น** | **default: 0** |
| `project_status` | `string` | **สถานะโปรเจค** | **default: paycheck** |
| `img_slip` | `file` | **รูปหลักฐานการชำระเงิน โฟรเดอร์สลิปแจ้งชำระเงินโปรเจค** |
| `tracking_number` | `string` | **เลขติดตามพัสดุกรณีมีการจัดส่ง** | **default: ""** |
| `express_brand` | `string` | **แบรนด์ขนส่ง** | **default: ""** |
| `timestamp` | `date` | **วันเวลาที่เริ่มโปรเจค** | **default: 0** |

### การลบข้อมูล art_work

```http
DELETE /:_id
_id=62860054821f7b69619f254
```
