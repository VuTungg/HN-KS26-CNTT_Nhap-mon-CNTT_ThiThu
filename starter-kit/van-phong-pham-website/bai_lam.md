# BÀI LÀM – THI THỬ HACKATHON 01

- **Mã đề:** Thi thử
- **Họ tên:Vũ Nam Tùng**
- **Lớp:CNTT3**
- **Link repository:**
- **Hệ điều hành (Windows/macOS):Windows**

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
pwd
ls -Force
mv .\nhap_hang.txt docs/
mv .\logo_van_phong_pham.png media/
cp .\media\logo_van_phong_pham.png .\backup\
rm .\temp_131.tmp
cd log
ls
cd ..
Get-ChildItem -Recurse -Force
Get-Content logs/shop.log | Select-String "ERROR" > logs/daily_report.txt
Get-Content logs/daily_report.txt
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
.\auto_report.ps1
Get-Content logs/auto_report.txt
(Get-Content logs/shop.log | Select-String "ERROR").Count
"=== TONG HOP LOG ===" > logs/tong_hop.txt
 Get-Content logs/shop.log | Select-String "WARNING" >> logs/tong_hop.txt
 Get-Content logs/shop.log | Select-String "ERROR").Count >> logs/tong_hop.txt
 Get-Content logs/tong_hop.txt
```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> pwd

Path
----
D:\starter-kit(3)\starter-kit\van-phong-pham-website


PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> ls -Force


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/23/2026   8:43 AM                backup
d-----        10/23/2026   8:46 AM                data
d-----        10/23/2026   8:43 AM                docs
d-----        10/23/2026   8:46 AM                logs
d-----        10/23/2026   8:43 AM                media
-a----        10/19/2026  10:00 AM           2253 bai_lam.md
-a----        10/19/2026   9:41 AM           6053 logo_van_phong_pham.png
-a----        10/19/2026   9:41 AM             51 nhap_hang.txt
------        10/19/2026   9:41 AM             22 temp_131.tmp


PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> mv .\nhap_hang.txt docs/
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> mv .\logo_van_phong_pham.png media/
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> cp .\media\logo_van_phong_pham.png .\backup\
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> rm .\temp_131.tmp
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> cd logs
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website\logs> ls


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           1053 shop.log


PS D:\starter-kit(3)\starter-kit\van-phong-pham-website\logs> cd ..
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> Get-ChildItem -Recurse -Force


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/23/2026   8:43 AM                backup
d-----        10/23/2026   8:46 AM                data
d-----        10/23/2026   8:49 AM                docs
d-----        10/23/2026   8:46 AM                logs
d-----        10/23/2026   8:49 AM                media
-a----        10/19/2026  10:00 AM           2253 bai_lam.md


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website\backup


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           6053 logo_van_phong_pham.png


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website\data


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           6105 don_ban_thang_10.xlsx


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website\docs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM             51 nhap_hang.txt


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           1053 shop.log


    Directory: D:\starter-kit(3)\starter-kit\van-phong-pham-website\media


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/19/2026   9:41 AM           6053 logo_van_phong_pham.png


PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> Get-Content logs/shop.log | Select-String "ERROR" > logs/daily_report.txt
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> Get-Content logs/daily_report.txt

2025-10-28 08:24:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:30:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:33:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:39:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:42:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 09:12:28 [ERROR] Thanh toan bi tu choi


PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> .\auto_report.ps1
Dang loc log...
Hoan thanh!
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> Get-Content logs/auto_report.txt
=== BAO CAO LOI ===

2025-10-28 08:24:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:30:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:33:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:39:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:42:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 09:12:28 [ERROR] Thanh toan bi tu choi


PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> (Get-Content logs/shop.log | Select-String "ERROR").Count
6
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> "=== TONG HOP LOG ===" > logs/tong_hop.txt
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> Get-Content logs/shop.log | Select-String "WARNING" >> logs/tong_hop.txt
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> (Get-Content logs/shop.log | Select-String "ERROR").Count >> logs/tong_hop.txt
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website> Get-Content logs/tong_hop.txt
=== TONG HOP LOG ===

2025-10-28 08:51:28 [WARNING] Thoi gian tai trang cham
2025-10-28 08:54:28 [WARNING] Anh san pham dung luong lon
2025-10-28 08:57:28 [WARNING] Thoi gian tai trang cham


6
PS D:\starter-kit(3)\starter-kit\van-phong-pham-website>

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
# Get-Content logs/daily_report.txt

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
2025-10-28 08:24:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:30:28 [ERROR] Thanh toan bi tu choi

```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [x] Heading 1: tên dự án
- [x] Mô tả ngắn có cả **in đậm** và _in nghiêng_
- [x] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [x] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [x] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [x] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# .\auto_report.ps1

```

### Nội dung file logs/auto_report.txt

```text
=== BAO CAO LOI ===

2025-10-28 08:24:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:30:28 [ERROR] Thanh toan bi tu choi
2025-10-28 08:33:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:39:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 08:42:28 [ERROR] Ket noi kho du lieu that bai
2025-10-28 09:12:28 [ERROR] Thanh toan bi tu choi



```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
# (Get-Content logs/shop.log | Select-String "ERROR").Count

```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
6

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
pwd
ls -Force
mv .\nhap_hang.txt docs/
mv .\logo_van_phong_pham.png media/
cp .\media\logo_van_phong_pham.png .\backup\
rm .\temp_131.tmp
cd log
ls
cd ..
Get-ChildItem -Recurse -Force
Get-Content logs/shop.log | Select-String "ERROR" > logs/daily_report.txt
Get-Content logs/daily_report.txt
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
.\auto_report.ps1
Get-Content logs/auto_report.txt
(Get-Content logs/shop.log | Select-String "ERROR").Count
"=== TONG HOP LOG ===" > logs/tong_hop.txt
 Get-Content logs/shop.log | Select-String "WARNING" >> logs/tong_hop.txt
 Get-Content logs/shop.log | Select-String "ERROR").Count >> logs/tong_hop.txt
 Get-Content logs/tong_hop.txt
```

### Nội dung file logs/tong_hop.txt

```text
=== TONG HOP LOG ===

2025-10-28 08:51:28 [WARNING] Thoi gian tai trang cham
2025-10-28 08:54:28 [WARNING] Anh san pham dung luong lon
2025-10-28 08:57:28 [WARNING] Thoi gian tai trang cham


6


```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/don_ban_thang_10.xlsx`, không cần ghi vào đây.
