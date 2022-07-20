# การเพิ่ม Point Happy-Point ผ่าน API

## https://happy-point.nbadigitalservice.com/api/happy-point/recived_point/commission

### การเพิ่มข้อมูล Point Happy Point

```http
post /
```

Body
| Parameter | Type | Description | ตัวอย่าง |
| :--- | :--- | :--- |:--- |
| `phone_number` | `string` | **เบอร์โทรศัพท์** | 0830936555
| `point` | `number` | **Point ทีได้รับ** | 8000
| `title` | `string` | **หัวข้อหลัก** | ค่าคอมมิสชั่น, ค่าเชิญชวน, ค่าสั่งซื้อสินค้า
| `detail` | `string` | **รายละเอียด** | ได้รับค่าคอมมิสชั่นจาก NBA Platform <br>ได้รับค่าคอมมิสชั่นงานเขียนเว็บของลูกทีม จาก NBA Platform, <br>ได้รับจากการสั่งซื้อสินค้า ของ FoodExpress
| `timestamp` | `date` | **วันที่ทำรายการ** | "2022-07-20T07:56:11.251+00:00" <br>
dayjs(Date.now()).format()
