# การเพิ่ม Point Happy-Point ผ่าน API

## https://happy-point.nbadigitalservice.com/api/happy-point/recived_point/change_point

### การเพิ่มข้อมูล Members Happy Point

```http
put /
```

Body
| Parameter | Type | Description |
| :--- | :--- | :--- |
| `phone_number` | `string` | **เบอร์โทรศัพท์** |
| `point` | `number` | **Point ทีได้รับ** |
