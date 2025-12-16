# 🏨 Hotel Management System – WinForms (C#)

- **Author**: Hồ Duy Vũ – Software Engineer | AI & Backend Developer
- **GitHub**: https://github.com/Ho-Duy-Vu
- **Email**: duyvu11092004@gmail.com
📌 **Project Type:** Desktop Application  

---

## 📌 Giới Thiệu

**Hotel Management System** là một ứng dụng quản lý khách sạn được phát triển bằng **C# WinForms**, nhằm hỗ trợ việc quản lý toàn diện các nghiệp vụ trong khách sạn như:

- Quản lý phòng
- Đặt phòng
- Quản lý khách hàng
- Quản lý nhân viên
- Quản lý hóa đơn & thanh toán

Dự án hướng tới việc **chuẩn hóa quy trình quản lý**, giảm sai sót thủ công và nâng cao hiệu quả vận hành khách sạn.

---

## 🎯 Mục Tiêu Dự Án

- Số hóa toàn bộ quy trình quản lý khách sạn
- Quản lý dữ liệu tập trung, chính xác
- Tăng hiệu suất làm việc của nhân viên
- Dễ sử dụng, phù hợp cho khách sạn vừa và nhỏ
- Áp dụng kiến thức **C#, WinForms, SQL Server** vào bài toán thực tế

---

## ✨ Tính Năng Chính

### 🛏️ Quản Lý Phòng

**Mục tiêu:**  
Theo dõi thông tin phòng, trạng thái sử dụng và tình trạng vệ sinh.

**Chức năng:**
- Thêm / sửa / xóa phòng
- Quản lý thông tin:
  - Loại phòng
  - Giá phòng
  - Số lượng giường
- Cập nhật trạng thái:
  - Trống
  - Đã đặt
  - Đang sử dụng (Check-in)
  - Đã trả phòng (Check-out)
- Tìm kiếm phòng theo:
  - Loại phòng
  - Giá tiền
  - Trạng thái

---

### 🏨 Quản Lý Đặt Phòng

**Mục tiêu:**  
Quản lý các đơn đặt phòng của khách hàng một cách chính xác.

**Chức năng:**
- Tiếp nhận yêu cầu đặt phòng
- Kiểm tra tình trạng phòng khả dụng
- Lưu thông tin đặt phòng:
  - Mã đặt phòng
  - Thông tin khách hàng
  - Thời gian nhận / trả phòng
  - Tiền cọc
- Tự động cập nhật trạng thái phòng từ **Trống → Đã đặt**

---

### 👤 Quản Lý Khách Hàng

**Mục tiêu:**  
Lưu trữ và quản lý thông tin khách hàng để hỗ trợ tốt hơn trong các lần giao dịch.

**Chức năng:**
- Đăng ký thông tin khách hàng:
  - Họ tên
  - Số điện thoại
  - Email
  - Địa chỉ
- Lưu lịch sử đặt phòng
- Tra cứu khách hàng theo:
  - Mã khách hàng
  - Thông tin cá nhân
- Hỗ trợ quản lý khách hàng thân thiết (mở rộng)

---

### 👨‍💼 Quản Lý Nhân Viên

**Mục tiêu:**  
Quản lý nhân sự và kiểm soát quyền truy cập hệ thống.

**Chức năng:**
- Thêm / cập nhật / xóa nhân viên
- Quản lý thông tin:
  - Họ tên
  - Số điện thoại
  - Giới tính
  - Email
- Quản lý tài khoản đăng nhập
- Phân quyền sử dụng hệ thống

---

### 🧾 Quản Lý Hóa Đơn & Thanh Toán

**Mục tiêu:**  
Quản lý quá trình thanh toán và xuất hóa đơn cho khách hàng.

**Chức năng:**
- Tính tiền phòng theo thời gian lưu trú
- Quản lý tiền cọc
- Lập hóa đơn thanh toán
- Lưu lịch sử giao dịch

---

## 🔄 Tích Hợp Quy Trình

Các phân hệ trong hệ thống được **liên kết chặt chẽ**:

- Trạng thái phòng tự động cập nhật từ module Đặt phòng
- Hồ sơ khách hàng được tạo/cập nhật khi phát sinh giao dịch
- Nhân viên đăng nhập hệ thống theo phân quyền được cấp

---

## 🛠️ Công Nghệ Sử Dụng

| Thành phần | Công nghệ |
|----------|----------|
| Ngôn ngữ | C# |
| Framework | WinForms |
| Database | SQL Server |
| UI | Windows Forms |
| IDE | Visual Studio |

---

## 📂 Cấu Trúc Dự Án (Tham Khảo)

```bash
WINFORM_QLKS/
│── DAL/            # Data Access Layer
│── BLL/            # Business Logic Layer
│── GUI/            # WinForms UI
│── Models/         # Entity / Model classes
│── Database/       # SQL scripts
│── app.config
│── Program.cs
│── README.md
