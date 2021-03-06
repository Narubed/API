# Members

## https://api.nbadigitalservice.com/v1/platform

### การดึงข้อมูลของ members ทั้งหมด

```http
GET /members
```

### การดึงข้อมูลของ members ผ่านไอดี

```http
GET /members/:_id
_id = 62860054821f7b69619f254
```

### การดึงข้อมูลของ members ผ่านเบอร์โทร

```http
GET /members/tel/:id
id = 0830930000
```

### การเพิ่มข้อมูล members

```http
POST /members
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `ref_id` | `string` | **รหัสผู้แนะนำ โดย เป็นค่า card_number ของสมาชิกคนอื่น** |
| `card_number` | `string` | **รหัสบัตรสมาชิก สร้างจาก เลข 888888+เบอร์โทร 10 หลัก (จะต้องไม่ซ้ำ)** |
| `mem_package` | `string` | **แพ็คเก็จที่สมัคร Platinum (ใหญ่สุด) Gold (กลาง) Silver (เริ่มต้น)** |
| `mem_name` | `string` | **ชื่อ-นามสกุล** |
| `mem_tel` | `string` | **เบอร์โทร (ใช้เป็นชื่อผู้ใช้งานเข้าระบบด้วย)** |
| `mem_password` | `string` | **รหัสผ่าน** |
| `mem_iden` | `file` | **รูปภาพบัตรประชาชน** |
| `img_iden` | `string` | **บัญชีธนาคาร** |
| `mem_bank` | `number` | **หมายเลขบัญชีธนาคาร** |
| `mem_bank_num` | `string` | **หมายเลขบัญชีธนาคาร**|
| `img_bank` | `file` | **รูปหน้าสมุดบัญชีธนาคาร**|
| `mem_address` | `string` | **ที่อยู่** |
| `mem_subdistrict` | `string` | **ตำบล** |
| `mem_district` | `string` | **อำเภอ** |
| `mem_province` | `string` | **จังหวัด** |
| `mem_start` | `date` | **วันที่เริ่มต้น** | **default: new Date()** |
| `mem_expire` | `date` | **วันหมดอายุ** | **default: new Date()** |
| `mem_money` | `number` | **ยอดเงินในกระเป๋า** | **default: 0** |
| `mem_credit` | `number` | **ยอดเงินสำหรับเก็บค่าคอมมิชชั่น หรือค่าแนะนำ** | **default: 0** |
| `mem_status` | `string` | **สถานะของสมาชิกที่สมัคร process อยู่ระหว่างการตรวจสอบ online ออนไลน์ offline ออฟไลน์ (บัญชีถูกปิดการใช้งาน)** | **default: process** |
| `mem_upline` | `array` | **ผู้ใช้งานที่อยู่สูงกว่า** | **default: []** |
| `mem_allsale` | `number` | **AllSale** | **default: 0** |

### การแก้ไขข้อมูล members

```http
PUT /members/:_id
_id=62860054821f7b69619f254
```

Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `ref_id` | `string` | **รหัสผู้แนะนำ โดย เป็นค่า card_number ของสมาชิกคนอื่น** |
| `card_number` | `string` | **รหัสบัตรสมาชิก สร้างจาก เลข 888888+เบอร์โทร 10 หลัก (จะต้องไม่ซ้ำ)** |
| `mem_package` | `string` | **แพ็คเก็จที่สมัคร Platinum (ใหญ่สุด) Gold (กลาง) Silver (เริ่มต้น)** |
| `mem_name` | `string` | **ชื่อ-นามสกุล** |
| `mem_tel` | `string` | **เบอร์โทร (ใช้เป็นชื่อผู้ใช้งานเข้าระบบด้วย)** |
| `mem_password` | `string` | **รหัสผ่าน** |
| `mem_iden` | `file` | **รูปภาพบัตรประชาชน** |
| `img_iden` | `string` | **บัญชีธนาคาร** |
| `mem_bank` | `number` | **หมายเลขบัญชีธนาคาร** |
| `mem_bank_num` | `string` | **หมายเลขบัญชีธนาคาร**|
| `img_bank` | `file` | **รูปหน้าสมุดบัญชีธนาคาร**|
| `mem_address` | `string` | **ที่อยู่** |
| `mem_subdistrict` | `string` | **ตำบล** |
| `mem_district` | `string` | **อำเภอ** |
| `mem_province` | `string` | **จังหวัด** |
| `mem_start` | `date` | **วันที่เริ่มต้น** | **default: new Date()** |
| `mem_expire` | `date` | **วันหมดอายุ** | **default: new Date()** |
| `mem_money` | `number` | **ยอดเงินในกระเป๋า** | **default: 0** |
| `mem_credit` | `number` | **ยอดเงินสำหรับเก็บค่าคอมมิชชั่น หรือค่าแนะนำ** | **default: 0** |
| `mem_status` | `string` | **สถานะของสมาชิกที่สมัคร process อยู่ระหว่างการตรวจสอบ online ออนไลน์ offline ออฟไลน์ (บัญชีถูกปิดการใช้งาน)** | **default: process** |
| `mem_upline` | `array` | **ผู้ใช้งานที่อยู่สูงกว่า** | **default: []** |
| `mem_allsale` | `number` | **AllSale** | **default: 0** |

### การลบข้อมูล members

```http
DELETE /members/:_id
_id=62860054821f7b69619f254
```

### การเพิ่มข้อมูล Credit

```http
PUT /members/add_credit/:_id
_id=62860054821f7b69619f254 (_id ของ members)
```

| Parameter     | Type     | Description       | Default |
| :------------ | :------- | :---------------- | :------ |
| `mem_credit`  | `number` | **จำนวนที่เพิ่ม** |
| `detail`      | `string` | **รายละเอียด**    |
| `mem_allsale` | `string` | **เพิม allsale**  |
| `timestamp`   | `date`   | **timestamp**     |

### การลบข้อมูล Credit

```http
PUT /members/minus_credit/:_id
_id=62860054821f7b69619f254 (_id ของ members)
```

| Parameter    | Type     | Description    | Default |
| :----------- | :------- | :------------- | :------ |
| `mem_credit` | `number` | **จำนวนที่ลบ** |
| `detail`     | `string` | **รายละเอียด** |
| `timestamp`  | `date`   | **timestamp**  |

### การเพิ่มข้อมูล wallet

```http
POST /members/add_wallet/

```

| Parameter    | Type     | Description       | Default |
| :----------- | :------- | :---------------- | :------ |
| `mem_id`     | `number` | **mem id**        |
| `mem_amount` | `number` | **จำนวนที่เพิ่ม** |
| `detail`     | `string` | **รายละเอียด**    |
| `timestamp`  | `date`   | **timestamp**     |

### การลบข้อมูล wallet

```http
POST /members/minus_wallet/
```

| Parameter    | Type     | Description       | Default |
| :----------- | :------- | :---------------- | :------ |
| `mem_id`     | `number` | **mem id**        |
| `mem_amount` | `number` | **จำนวนที่เพิ่ม** |
| `detail`     | `string` | **รายละเอียด**    |
| `timestamp`  | `date`   | **timestamp**     |


### การลบข้อมูล allsela
```http
POST /members/minus_allsela/
```

| Parameter    | Type     | Description       | Default |
| :----------- | :------- | :---------------- | :------ |
| `mem_id`     | `number` | **mem id**        |
| `amount` | `number` | **จำนวนที่ลบ** |
| `detail`     | `string` | **รายละเอียด**    |
| `timestamp`  | `date`   | **timestamp**     |
