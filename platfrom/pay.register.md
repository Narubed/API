# pay_register (การเบิกเงินล่วงหน้า)

## https://api.nbadigitalservice.com/v1/platform

### การดึงข้อมูลของ pay_register ทั้งหมด

```http
GET /pay_register
```

### การดึงข้อมูลของ pay_register ผ่านไอดี

```http
GET /pay_register/:_id
_id=62860054821f7b69619f254
```

### การเพิ่มข้อมูล pay_register

```http
POST /pay_register
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `pay_type` | `string` | **ประเภทการชำระ** |**default: slip**|
| `mem_id` | `string` | **จาก _id ในตาราง member** |
| `amount` | `number` | **ยอดที่โอนโดยอ้างอิงจาก แพ็คเก็จที่สมัคร** |
| `img_slip` | `file` | **รูปหลักฐานการโอนเงิน** |
| `pay_status` | `date` | **สถานะ process success** |**default: process** |
| `pay_timestamp` | `date` | **วันที่ทำรายการ** |**default: new Date()** |

### การแก้ไขข้อมูล pay_register

```http
PUT /pay_register/:_id
_id=62860054821f7b69619f254
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `avm_owner` | `string` | **\_id เจ้าของรายงาน** |
| `avm_amount` | `number` | **จำนวนเงิน** |
| `avm_status` | `string` | **สถานะรายงาน** | **default: waiting**|
| `avm_timestamp` | `date` | **วันที่ทำรายการ** |**default: new Date()** |

### การลบข้อมูล pay_register

```http
DELETE /pay_register/:_id
_id=62860054821f7b69619f254
```
