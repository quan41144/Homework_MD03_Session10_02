## TH1: Người dùng gửi yêu cầu đặt lịch khám nhưng bỏ trống tên bệnh nhân.
* mã lỗi HTTP phù hợp: 400 - Bad Request
### => Giải thích: Vì đây là lỗi do lỗi cú dữ liệu đầu vào từ phía Client.
## TH2: Tìm kiếm hồ sơ bệnh án với ID là 999 nhưng trong Database không tồn tại.
* mã lỗi HTTP phù hợp: 404 - Not Found
### => Giải thích: Vì đây là lỗi do phía Client nhập URL trỏ đến id của hồ sơ bệnh án nhưng lại không có trong database.
## TH3: Hệ thống đang chạy thì Database MySQL bị sập, không thể truy vấn dữ liệu.
* mã lỗi HTTP phù hợp: 500 - Internal Server Error
### => Giải thích: Vì đây là lỗi của phía Server, dù Client gửi đúng yêu cầu nhưng Server không thể xử lý.
## TH4: Người dùng nhập tuổi bệnh nhân là -5 (Dữ liệu không hợp lệ về mặt logic).
* mã lỗi HTTP phù hợp: 400 - Bad Request
### => Giải thích: Vì đây là lỗi logic dữ liệu đầu vào từ phía Client.