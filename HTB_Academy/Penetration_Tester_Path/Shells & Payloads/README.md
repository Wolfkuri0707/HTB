# Lời giải — Shells & Payloads

### Q1: Which two shell languages did we experiment with in this section? (Format: shellname&shellname)


![Answer](./images/pic1.jpg)

> **Đáp án:** `bash&powershell`

---

### Q2: In Pwnbox issue the $PSversiontable variable using PowerShell. Submit the edition of PowerShell that is running as the answer.

Chạy lệnh: `$PSversiontable`

![Nmap Scan](./images/pic2.jpg)

> **Đáp án:** `Core`

---

### Q3: Des is able to issue the command nc -lvnp 443 on a Linux target. What port will she need to connect to from her attack box to successfully establish a shell session?


Nhìn trên câu hỏi ta đã thấy cổng kết nối là 443

> **Đáp án:** `443`

---

### Q4: SSH to the target, create a bind shell, then use netcat to connect to the target using the bind shell you set up. When you have completed the exercise, submit the contents of the flag.txt file located at /customscripts.

Đầu tiên dựa theo `IP` `username` `password` đã được cung cấp, ta tiến hành SSH  
`ssh <username>@<IP>`

![SSH](./images/pic3.jpg)

Mở 1 terminal khác, terminal này sẽ để netcat vào máy mục tiêu thông qua cổng 4444  
`nc -nv <IP> 444`

![Catch](./images/pic4.jpg)

Sau khi bắt được tín hiệu từ cổng 4444, ta đã truy cập thành công vào máy chủ

![Cat_Answer](./images/pic5.jpg)

Lấy đáp án

> **Đáp án:** `B1nD_Shells_r_cool`

---

### Q5: When establishing a reverse shell session with a target, will the target act as a client or server?

`Máy tấn công (máy mình)` là máy lắng nghe là `máy nhận thông tin` tương đương `server`, còn máy target là máy truyền thông tin nên là máy `client`

> **Đáp án:** `client`

---

