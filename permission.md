1
IOS:

- Quyền sử dụng Camera

- Quyền Truy cập photo

- Quyền truy cập Lịch

- Quyền truy cập FaceID

- Quyền truy cập Liên hệ, contact

Android:

- Quyền sử dụng biomaetrics

- Quyền sử dụng vân tay

- Quyền Internet, trạng thái mạng

- Quyền sử dụng Rung , Camera ,Đọc lịch, Viết lịch

- Quyền ghi vào bộ nhớ, Đọc bộ nhớ, đọc lịch, viết lịch

- Quyền tải xuống không có thông báo

2
Khai báo permission để xin quyền từ người dùng, thông báo cho người dùng biết App cần dùng những gì trong máy, và cần được cấp quyền để sử dụng chúng.

Không khai báo permission sẽ không thể dùng được tính năng hoặc bị crash app

3
Trong Android Studio, nội dung của hộp thoại yêu cầu quyền (permission dialog) là một phần của hệ thống điều hành Android và không thể điều chỉnh từ Android Studio.
Nội dung của hộp thoại này phụ thuộc vào loại quyền mà ứng dụng yêu cầu và thiết lập của hệ thống điều hành.

    Trong Xcode, nội dung trong popup permission có thể được điều chỉnh tùy theo mục đích sử dụng của ứng dụng và theo các quy định của hệ điều hành.
    ```
        <key>NSCameraUsageDescription</key>
        <string>Ứng dụng cần truy cập camera để chụp ảnh và quay video.</string>
    ```

4
Trong Android mọi giao diện người dùng do hệ thống cung cấp,hộp thoại cấp phép, sẽ sử dụng ngôn ngữ do người dùng chọn cho thiết bị của họ, không thể thay đổi hoặc can thiệp đến popup mà nó cung cấp
Trong xcode có thể custom được message đa ngôn ngữ nhưng người dùng phải chọn ngôn ngữ trong phần cài đặt của máy, hệ thống sẽ tự chuyển ngôn ngữ trong app nếu app có sử dụng Localizations để support cho từng ngôn ngữ đó

Full list permisstion IOS:

```
Full List:

Apple Music:

<key>NSAppleMusicUsageDescription</key>
<string>My description about why I need this capability</string>
Bluetooth:

<key>NSBluetoothPeripheralUsageDescription</key>
<string>My description about why I need this capability</string>
Calendar:

<key>NSCalendarsUsageDescription</key>
<string>My description about why I need this capability</string>
Camera:

<key>NSCameraUsageDescription</key>
<string>My description about why I need this capability</string>
Contacts:

<key>NSContactsUsageDescription</key>
<string>My description about why I need this capability</string>
FaceID:

<key>NSFaceIDUsageDescription</key>
<string>My description about why I need this capability</string>
Health Share:

<key>NSHealthShareUsageDescription</key>
<string>My description about why I need this capability</string>
Health Update:

<key>NSHealthUpdateUsageDescription</key>
<string>My description about why I need this capability</string>
Home Kit:

<key>NSHomeKitUsageDescription</key>
<string>My description about why I need this capability</string>
Location:

<key>NSLocationUsageDescription</key>
<string>My description about why I need this capability</string>
Location (Always):

<key>NSLocationAlwaysUsageDescription</key>
<string>My description about why I need this capability</string>
Location (When in use):

<key>NSLocationWhenInUseUsageDescription</key>
<string>My description about why I need this capability</string>
Microphone:

<key>NSMicrophoneUsageDescription</key>
<string>My description about why I need this capability</string>
Motion (Accelerometer):

<key>NSMotionUsageDescription</key>
<string>My description about why I need this capability</string>
NFC (Near-field communication):

<key>NFCReaderUsageDescription</key>
<string>My description about why I need this capability</string>
Photo Library:

<key>NSPhotoLibraryUsageDescription</key>
<string>My description about why I need this capability</string>
Photo Library (Write-only access):

<key>NSPhotoLibraryAddUsageDescription</key>
<string>My description about why I need this capability</string>
Reminders:

<key>NSRemindersUsageDescription</key>
<string>My description about why I need this capability</string>
Siri:

<key>NSSiriUsageDescription</key>
<string>My description about why I need this capability</string>
Speech Recognition:

<key>NSSpeechRecognitionUsageDescription</key>
<string>My description about why I need this capability</string>
```

Full list permissions Android :

```
Dưới đây là danh sách các permission được sử dụng trong Android:

android.permission.READ_CALENDAR: Truy cập lịch của người dùng.

android.permission.WRITE_CALENDAR: Sửa đổi lịch của người dùng.

android.permission.CAMERA: Truy cập camera của thiết bị.

android.permission.READ_CONTACTS: Truy cập danh bạ của người dùng.

android.permission.WRITE_CONTACTS: Sửa đổi danh bạ của người dùng.

android.permission.GET_ACCOUNTS: Truy cập danh sách tài khoản của người dùng.

android.permission.ACCESS_FINE_LOCATION: Truy cập vị trí chính xác của thiết bị.

android.permission.ACCESS_COARSE_LOCATION: Truy cập vị trí xấp xỉ của thiết bị.

android.permission.RECORD_AUDIO: Ghi âm âm thanh từ micro của thiết bị.

android.permission.READ_PHONE_STATE: Truy cập trạng thái điện thoại, bao gồm cả IMEI của thiết bị.

android.permission.CALL_PHONE: Thực hiện cuộc gọi từ thiết bị.

android.permission.READ_CALL_LOG: Truy cập lịch sử cuộc gọi của thiết bị.

android.permission.WRITE_CALL_LOG: Sửa đổi lịch sử cuộc gọi của thiết bị.

android.permission.ADD_VOICEMAIL: Thêm tin nhắn thoại mới vào hộp thư thoại thoại của thiết bị.

android.permission.USE_SIP: Sử dụng giao thức SIP để thực hiện cuộc gọi thoại.

android.permission.PROCESS_OUTGOING_CALLS: Lắng nghe sự kiện của các cuộc gọi đi ra để thực hiện các hành động nhất định.

android.permission.BODY_SENSORS: Truy cập các cảm biến trên cơ thể như nhịp tim, nhiệt độ, áp lực máu, v.v.

android.permission.SEND_SMS: Gửi tin nhắn văn bản từ thiết bị.

android.permission.RECEIVE_SMS: Nhận tin nhắn văn bản trên thiết bị.

android.permission.READ_SMS: Truy cập tin nhắn văn bản trên thiết bị.

android.permission.RECEIVE_WAP_PUSH: Nhận các thông báo WAP Push từ nhà cung cấp dịch vụ.

android.permission.RECEIVE_MMS: Nhận tin nhắn MMS trên thiết bị.

android.permission.READ_EXTERNAL_STORAGE: Truy cập dữ liệu lưu trữ bên ngoài trên thiết bị.

android.permission.WRITE_EXTERNAL_STORAGE: Sửa đổi dữ liệu lưu trữ bên ngoài trên thiết bị.
```
