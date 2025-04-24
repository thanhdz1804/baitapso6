# baitapso6 :Hệ quản trị CSDL
Chủ đề: Câu lệnh Select
Yêu cầu bài tập: 
Cho file sv_tnut.sql (1.6MB)
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)
DEADLINE: 23H59:59 NGÀY 25/4/2025
Ghi chú: Giải thích tại sao lại có SQL như vậy.
## Các bước để import
### Bước 1: tạo database để chứa dữ liệu
![image](https://github.com/user-attachments/assets/62477d18-c045-4ac8-90b3-e66d352e2294)
### Bước 2: Mở file sv_tnut.sql trong 
![image](https://github.com/user-attachments/assets/36173884-f895-4ea2-b151-8639790d1045)
### Bước 3: Thực thi file script
![image](https://github.com/user-attachments/assets/6bb52989-8d6f-4dda-b1c1-d22ad1438353)
Bấm Execute (hoặc nhấn F5) để chạy toàn bộ script.
### Bước 4: Kiểm tra kết quả
Mở lại phần Object Explorer bên trái.
Mở thư mục Tables để kiểm tra các bảng đã được tạo.
Chuột phải vào bảng → Select Top 1000 Rows để xem dữ liệu đã được import chưa.
![image](https://github.com/user-attachments/assets/f7e9bb4a-7b15-494a-be46-8d5130682f00)
## Dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên
![image](https://github.com/user-attachments/assets/a5ceef0c-df11-463f-a9b5-0bf12f573100)
## Nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
![image](https://github.com/user-attachments/assets/a44ecd73-ff27-4ce4-ad79-037877e08961)
## Nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
![image](https://github.com/user-attachments/assets/09bb3121-ad00-4c8d-a698-ffecbfe21121)
## Nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
![image](https://github.com/user-attachments/assets/31a117b7-97d2-4056-9dc6-9e395754948a)
## Nhập sql để tìm xem có những sv nào trùng tên với em?
![image](https://github.com/user-attachments/assets/f140359b-6dfd-49ee-97c2-cfdf947fc879)
## Nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em
![image](https://github.com/user-attachments/assets/27778c30-c9c9-470e-9b8a-e874de13b913)
##  Nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
![image](https://github.com/user-attachments/assets/5ee21370-6eed-4396-94bc-f88198258ebc)
## BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
SELECT *	Lấy tất cả các cột từ bảng SV.
FROM SV	Lấy dữ liệu từ bảng SV.
WHERE nganh = 'KMT'	Chỉ chọn các sinh viên thuộc ngành "KMT" (có thể là Khoa học Máy tính, Kỹ thuật Máy tính...).
ORDER BY ten, hodem	Sắp xếp theo tên trước, sau đó đến họ đệm.
COLLATE Vietnamese_CI_AS	Áp dụng quy tắc sắp xếp theo tiếng Việt có phân biệt trọng âm, để đúng thứ tự bảng chữ cái Việt Nam (phân biệt a, ă, â, e, ê, i, o, ô, ơ, u, ư, y...).
![image](https://github.com/user-attachments/assets/a8f88658-5c77-463b-9510-252e0cd0d4a1)
##
