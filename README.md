# Telegram-ESP32-CAM-Take-and-Send-Photo

được tôi tổng hợp dịch sang tiếng việt.link gốc :https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/
 và https://randomnerdtutorials.com/telegram-esp32-cam-photo-arduino/

1.Tạo bot Telegram:
Mở Telegram và làm theo các bước tiếp theo để tạo Telegram Bot. Đầu tiên, hãy tìm kiếm "botfather"
nhấp vào nút bắt đầu.
Nhập /newbot và làm theo hướng dẫn để tạo bot của bạn. Đặt tên và tên người dùng.
Nếu bot của bạn được tạo thành công, bạn sẽ nhận được tin nhắn có liên kết để truy cập bot và mã thông báo bot. Lưu mã thông báo bot vì bạn sẽ cần nó để ESP32 có thể tương tác với bot.

2.Nhận ID người dùng Telegram :
tìm kiếm "IDBot" 
Bắt đầu cuộc trò chuyện với bot đó và nhập /getid. Bạn sẽ nhận được trả lời lại với ID người dùng của mình. Lưu ID người dùng đó, bởi vì bạn sẽ cần nó ở phần sau của hướng dẫn này

3.Để cài đặt bảng ESP32 trong Arduino IDE của bạn, hãy làm theo các hướng dẫn tiếp theo sau:
Trong Arduino IDE của bạn, hãy chuyển đến File> Preferences
Nhập thông tin sau vào trường "Additional Board Manager URLs":
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
Sau đó, nhấp vào nút "OK":
Cài đặt ESP32 Add-on trong Arduino IDE Windows, Mac OS X, Linux nhập URL
Lưu ý: nếu bạn đã có URL bảng ESP8266, bạn có thể phân tách các URL bằng dấu phẩy như sau:
https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json, http://arduino.esp8266.com/stable/package_esp8266com_index.json
Mở Trình quản lý bảng. Đi tới  Tools > Board > Boards Manager…
Tìm kiếm ESP32 và nhấn nút cài đặt cho "ESP32 by Espressif Systems":
Nó sẽ được cài đặt sau vài giây.

4.Thư viện Bot Telegram toàn cầu:
https://github.com/witnessmenow/Universal-Arduino-Telegram-Bot/archive/master.zip
Đi tới Sketch > include Library > Add.ZIP Library...
Thêm thư viện bạn vừa tải xuống.

5.Thư viện ArduinoJson
cài đặt thư viện ArduinoJson. Làm theo các bước tiếp theo để cài đặt thư viện.
Đi tới Sketch > Include Library > Manage Libraries.
Tìm kiếm "ArduinoJson".
Cài đặt thư viện.
