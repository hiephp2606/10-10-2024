# Platform IO: ESP32 LDR
By Đào Ngọc Quý

## Mục đích : 
- Nâng cao sự nhanh nhẹn trong các quy trình làm việc với PlatformIO, Git và Github
- Sử dụng ESP32 để đo cường độ ánh sáng từ một quang trở (LDR)

## Yêu cầu :
- Đọc giá trị độ sáng (tương đối) từ quang trở qua chân ADC.
- In giá trị này ra cổng UART dưới dạng số nguyên (0 - 4095).
- Sử dụng công cụ Teleplot để vẽ đồ thị của cường độ ánh sáng theo thời gian thực.

## Phần cứng :
- Sử dụng board phát triển ESP32 Devkit v1
- Quang trở, điện trở và dây nối được kết nối như trong bài giảng 

## Hướng dẫn kết nối : 
-  Kết nối một chân của quang trở (LDR) với chân ADC (ví dụ: GPIO 34) của ESP32.
-  Kết nối chân còn lại của quang trở với nguồn 3.3V.
-  Kết nối một điện trở từ chân ADC đến GND.
-  Đảm bảo tất cả các kết nối chắc chắn.

## Hình ảnh đồ thị :
https://github.com/Daoquy14092003/ESP32_LDR_Test/blob/main/Plot1_LDR_Test.jpg?raw=true

## Hướng dẫn thêm : Cách chèn ảnh chụp màn hình đồ thị ánh sáng vào tệp README.md
- Tải ảnh lên GitHub: Mở repo trên Github, nhấn vào nút Add file và chọn Upload files, chọn tệp từ máy tính, nhấn Commit changes sau khi tải ảnh lên.
- Lấy đường dẫn của ảnh : Nhấp chuột phải vào ảnh và chọn Copy image address để sao chép đường dẫn của ảnh.

## Các công cụ trong `workspace` này
- Teleplot: Là một công cụ vẽ đồ thị trực quan, có thể hiển thị dữ liệu theo thời gian thực từ ESP32 qua cổng UART.
  Sử dụng để vẽ đồ thị cường độ ánh sáng được đọc từ LDR, giúp theo dõi và phân tích dữ liệu một cách trực quan.
- Sử dụng các thư viện có sẵn 
