# 💰 WEBSITE QUẢN LÝ CHI TIÊU CÁ NHÂN (PERSONAL FINANCE MANAGEMENT)

> [cite_start]**Đồ án môn học:** Chuyên đề ASP.NET (Học kỳ III, Năm học 2025-2026) 
> [cite_start]**Đơn vị thực hiện:** Trường Kỹ thuật và Công nghệ - Khoa Công nghệ Thông tin - Đại học Trà Vinh.

---

## 👥 THÔNG TIN ĐỘI NGŨ THỰC HIỆN

### [cite_start]Đội ngũ Sinh viên thực hiện (Lớp: DK24TT8016):
1. [cite_start]**Trương Lữ Quốc** (Nhóm trưởng) - **MSSV:** 170124186 
2. [cite_start]**Lê Tuấn Anh** - **MSSV:** 170124188 
3. [cite_start]**Hồ Trung Hiếu** - **MSSV:** 170124190 

### Giảng viên hướng dẫn:
* **TS. [cite_start]Đoàn Phước Miền** 

---

## 💻 CÔNG NGHỆ SỬ DỤNG

[cite_start]Hệ thống được phát triển toàn diện dựa trên mô hình kiến trúc **Client - Server** và mô hình **MVC (Model-View-Controller)** giúp tách biệt rõ ràng giữa các tầng dữ liệu, xử lý nghiệp vụ backend và hiển thị front-end[cite: 23]:

* [cite_start]**Backend:** `C#` (Ngôn ngữ lập trình hướng đối tượng cốt lõi) kết hợp với nền tảng `.NET SDK 8.0` & `ASP.NET Core MVC`[cite: 1, 11, 22].
* **Database (Cơ sở dữ liệu):** `Microsoft SQL Server Express (2022+)` xử lý quan hệ logic dữ liệu tài chính tối ưu thông qua các ràng buộc toàn vẹn[cite: 1, 12, 22, 25].
* [cite_start]**Front-end / UI:** `Bootstrap Framework` (Hệ thống lưới Grid System Responsive), `HTML5`, `CSS3`, `JavaScript` cùng hệ thống biểu đồ trực quan hóa dữ liệu dòng tiền[cite: 12, 24].
* [cite_start]**Công cụ phát triển:** `Visual Studio 2022` và `SQL Server Management Studio (SSMS)`[cite: 1, 13].

---

## 🛠️ CÁC CHỨC NĂNG QUAN TRỌNG

[cite_start]Hệ thống cung cấp giải pháp tài chính số hóa giúp chuẩn hóa và theo dõi dòng tiền qua 4 phân hệ thực thể cốt lõi (`tblTaiKhoan`, `tblVi`, `tblNganSach`, `tblGiaoDich`)[cite: 25, 29]:

1. [cite_start]**Phân hệ Quản lý Tài khoản (Bảo mật):** Đăng ký, Đăng nhập, Thay đổi thông tin cá nhân và Đổi mật khẩu[cite: 14, 53]. [cite_start]Cơ chế bảo mật băm mật khẩu (`PasswordHash`) giúp bảo vệ thông tin định danh và phân tách không gian lưu trữ biệt lập giữa từng người dùng[cite: 25, 54].
2. [cite_start]**Phân hệ Quản lý Ví tiền (Đa nguồn lưu trữ):** Cho phép người dùng khởi tạo và theo dõi biến động số dư thực tế theo từng loại nguồn tiền riêng biệt: Tiền mặt, Tài khoản ngân hàng, Ví điện tử (MoMo, Zalopay, v.v.)[cite: 21, 26, 449].
3. [cite_start]**Phân hệ Thiết lập Ngân sách (Hạn mức chi tiêu):** Thiết lập các giới hạn, chu kỳ chi tiêu theo từng danh mục cụ thể (như ăn uống, giáo dục, giải trí) nhằm đưa ra cảnh báo hoặc quản lý hành vi mua sắm vượt ngưỡng[cite: 27, 38, 61].
4. [cite_start]**Phân hệ Nhật ký Giao dịch (Thu / Chi):** Ghi chép chi tiết các khoản thu - chi hằng ngày, ràng buộc chặt chẽ với từng Tài khoản và Ví tiền tương ứng để tự động cập nhật, tính toán dòng tiền tăng/giảm tự động[cite: 28, 56].
5. [cite_start]**Bảng điều khiển trung tâm (Dashboard & Thống kê):** Trực quan hóa số liệu tài chính thông qua hệ thống biểu đồ thông minh: Biểu đồ cột biểu thị xu hướng Thu - Chi theo tháng, và Biểu đồ tròn thể hiện tỷ trọng danh mục chi tiêu, giúp người dùng nhận diện thói quen tiêu dùng tức thời[cite: 30, 14, 503].

---

## 🖼️ HÌNH ẢNH MINH HỌA DỰ ÁN

[cite_start]*Dưới đây là danh sách các hình ảnh giao diện thực tế của hệ thống được trích xuất từ tài liệu đồ án[cite: 16, 17, 18]:*

### 1. Kiến trúc hệ thống & Cơ sở dữ liệu
* **Sơ đồ Use Case tổng quan:**
  ![Sơ đồ Use Case](https://raw.githubusercontent.com/170124186-cmd/ASPNET-DK24TT8016-truongluquoc-qlchitieucanhan/main/images/use_case.png)
* **Sơ đồ thực thể cơ sở dữ liệu (Database Diagram):**
  ![Sơ đồ Cơ sở dữ liệu](https://raw.githubusercontent.com/170124186-cmd/ASPNET-DK24TT8016-truongluquoc-qlchitieucanhan/main/images/database_diagram.png)

### 2. Giao diện chức năng chính
* **Trang chủ hệ thống (Landing Page):**
  ![Giao diện Trang chủ](https://raw.githubusercontent.com/170124186-cmd/ASPNET-DK24TT8016-truongluquoc-qlchitieucanhan/main/images/trang_chu.png)
* **Bảng điều khiển & Biểu đồ Thống kê (Dashboard):**
  ![Giao diện Thống kê](https://raw.githubusercontent.com/170124186-cmd/ASPNET-DK24TT8016-truongluquoc-qlchitieucanhan/main/images/thong_ke.png)
* **Nhật ký Quản lý và dòng tiền Giao dịch:**
  ![Giao diện Giao dịch](https://raw.githubusercontent.com/170124186-cmd/ASPNET-DK24TT8016-truongluquoc-qlchitieucanhan/main/images/giao_dich.png)
* **Giao diện danh sách Ví tiền cá nhân:**
  ![Giao diện Quản lý Ví](https://raw.githubusercontent.com/170124186-cmd/ASPNET-DK24TT8016-truongluquoc-qlchitieucanhan/main/images/danh_sach_vi.png)
* **Giao diện Thiết lập Ngân sách:**
  ![Giao diện Ngân sách](https://raw.githubusercontent.com/170124186-cmd/ASPNET-DK24TT8016-truongluquoc-qlchitieucanhan/main/images/ngan_sach.png)

*(Lưu ý: Để hiển thị hình ảnh trên, bạn hãy tạo một thư mục mang tên `images` ở thư mục gốc của kho lưu trữ Github, sau đó tải các ảnh giao diện lên và đặt tên tương ứng: `use_case.png`, `database_diagram.png`, `trang_chu.png`, `thong_ke.png`, v.v.)*

---

## 🚀 HƯỚNG DẪN CÀI ĐẶT VÀ KHỞI CHẠYỨNG DỤNG

### 1. Yêu cầu hệ thống trước khi cài đặt
* [cite_start]Đảm bảo máy tính đã cài đặt sẵn **.NET SDK 8.0**.
* [cite_start]Cài đặt **Microsoft SQL Server 2022** (Khuyến nghị bản Express) kèm **SQL Server Management Studio (SSMS)**[cite: 1, 13].
* Công cụ IDE lập trình **Visual Studio 2022**[cite: 1, 13].

### 2. Các bước cài đặt chi tiết

#### Bước 1: Khởi tạo Cơ sở dữ liệu
1. Mở **SQL Server Management Studio (SSMS)** và kết nối vào SQL Server local của bạn.
2. Mở file script `database.sql` đính kèm trong dự án (Hoặc tạo `New Query` và dán toàn bộ nội dung script vào).
3. Nhấn **Execute (F5)** để khởi chạy tạo tự động cấu trúc cơ sở dữ liệu `chitieucanhanDB` và các dữ liệu thử nghiệm.

#### Bước 2: Cấu hình chuỗi kết nối (Connection String)
1. Di chuyển vào thư mục dự án chứa mã nguồn `src/` và mở tệp `appsettings.json`.
2. Tìm và điều chỉnh đường dẫn tên máy chủ `Server` tại mục `ConnectionStrings` sao cho phù hợp với máy của bạn:
   ```json
   "ConnectionStrings": {
     "DefaultConnection": "Server=.\\SQLEXPRESS;Database=chitieucanhanDB;Trusted_Connection=True;TrustServerCertificate=True;MultipleActiveResultSets=true"
   }
