1 IOS:

    Quyền sử dụng Camera

    Quyền Truy cập photo

    Quyền truy cập Lịch

    Quyền truy cập FaceID

    Quyền truy cập Liên hệ, contact

    Android:

    Quyền sử dụng biomaetrics

    Quyền sử dụng vân tay

    Internet, trạng thái mạng, Rung, ghi vào bộ nhớ, camera, đọc bộ nhớ,đọc lịch, viết lịch, tải xuống không có thông báo

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
