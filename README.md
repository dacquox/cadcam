# STM32F411 & ESP8266 Development Board — CAD/CAM

## Tổng quan thiết kế

- **Vi điều khiển chính:** STM32F411CEU6 (ARM Cortex-M4).
- **Kết nối không dây:** ESP-12F (ESP8266 Wi-Fi).
- **Giao tiếp với máy tính:** cổng USB Type-C và IC chuyển đổi USB–UART thuộc họ CH340.
- **Bộ nhớ ngoài:** Flash SPI W25Q128JVSIQ (128 Mbit) và khe thẻ SD.
- **Nguồn:** cấp nguồn từ đường 5 V, sử dụng AMS1117-3.3 tạo nguồn 3,3 V cho các khối phù hợp.
- **Dao động:** thạch anh 25 MHz và 32,768 kHz.
- **Điều khiển và mở rộng:** nút nhấn, LED báo trạng thái, đầu nối I/O và các tín hiệu SWD để lập trình/gỡ lỗi STM32.

## Các linh kiện chính

| Khối chức năng | Linh kiện | Vai trò |
| --- | --- | --- |
| Vi điều khiển | STM32F411CEU6 | Xử lý trung tâm |
| Wi-Fi | ESP-12F (ESP8266) | Kết nối mạng không dây |
| USB–UART | CH340 (U3) | Giao tiếp UART với máy tính |
| Ổn áp | AMS1117-3.3 | Tạo đường nguồn 3,3 V |
| Flash ngoài | W25Q128JVSIQ | Lưu trữ dữ liệu qua giao tiếp SPI |
| Thẻ nhớ | SDCARD | Giao tiếp với thẻ nhớ ngoài |
| USB | USB4105-GF-A | Đầu nối USB Type-C |
| Dao động | X1: 25 MHz; X2: 32,768 kHz | Tạo nguồn xung nhịp theo thiết kế |
| Ngoại vi | 4 LED, 4 nút nhấn, các header | Hiển thị, điều khiển và mở rộng |

## Nội dung đã thực hiện

- Xây dựng sơ đồ nguyên lý cho các khối MCU, Wi-Fi, nguồn, USB–UART, Flash và thẻ SD.
- Lựa chọn linh kiện, thiết lập symbol/footprint và bố trí linh kiện trên PCB.
- Thiết kế, đi dây và tổ chức các kết nối tín hiệu/nguồn trên PCB trong Altium Designer.
- Bố trí đầu nối mở rộng, nút nhấn và LED để thuận tiện cho phát triển phần mềm nhúng.
