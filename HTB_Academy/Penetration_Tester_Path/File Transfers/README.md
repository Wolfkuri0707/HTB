# Lời giải — File Transfers Module

### Q1: Download the file flag.txt from the web root using wget from the Pwnbox. Submit the contents of the file as your answer.

Dùng lệnh `wget http://<IP>/flag.txt`

![Wget](./images/pic2.jpg)

> **Đáp án:** `b1a4ca918282fcd96004565521944a3b`

---

### Q2: Upload the attached file named upload_win.zip to the target using the method of your choice. Once uploaded, unzip the archive, and run "hasher upload_win.txt" from the command line. Submit the generated hash as your answer.

Đề bài gợi ý chúng ta kết nối với máy chủ thông qua giao thức `RDP`, thông qua `username` và `password` đã được cung cấp  
do đang chạy trên máy ảo `kali linux` nên dùng lệnh: `xfreerdp /v:<IP> /u:<username> /p:<password> /cert:ignore +clipboard /dynamic-resolution`  
`/cert:ignore`: Bỏ qua xác thực chứng chỉ SSL  
`+clipboard`: Bật đồng bộ clipboard cho phép chia sẻ dữ liệu giữa các client
`/dynamic-resolution`: Tự động thay đổi độ phân giải để dễ nhìn

![RDP_client](./images/pic3.jpg)

Màn hình client hiện ra sau khi kết nối thành công

![connect_successfully](./images/pic4.jpg)

`hasher upload_win.txt`: tiến hành tạo ra mã băm cho file

![Hash_file](./images/pic6.jpg)


> **Đáp án:** `f458303ea783c224c6b4e7ef7f17eb9d`

---

### Q3: Download the file flag.txt from the web root using Python from the Pwnbox. Submit the contents of the file as your answer.

Lệnh `wget http://<IP>/flag.txt` để lấy đáp án

![Wget](./images/pic7.jpg)

> **Đáp án:** `5d21cf3da9c0ccb94f709e2559f3ea50`

---

