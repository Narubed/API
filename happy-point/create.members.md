# การสร้าง Members Happy-Point ผ่าน API

## https://happy-point.nbadigitalservice.com/api/happy-point/recived_point/

### การเพิ่มข้อมูล Members Happy Point

```http
POST /
```
Body
| Parameter | Type | Description | Default |
| :--- | :--- | :--- | :--- |
| `member_phone_number` | `string` | **เบอร์โทรศัพท์** |
| `member_firstname` | `string` | **ชื่อจริง** |
| `member_lastname` | `string` | **นามสกุล** |
| `member_address` | `string` | **ที่อยู่** |
| `member_password` | `string` | **รหัสผ่าน** |
| `member_current_point` | `number` | **จำนวน Point** |
| `member_total_point` | `number` | **จำนวน EXP หรือค่่าประสบการณ์** |
| `member_timestamp` | `date` | **วันที่สร้างผู้ใช้งาน** |
