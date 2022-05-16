***

Cho file bảng điểm chi tiết của các học sinh trong lớp các môn học liên quan đến việc thi đại học: Toán, Lý, Hóa, Sinh, Văn, Anh, Sử, Địa. Mỗi một môn học tự nhiên có 4 đầu điểm: Điểm kiểm tra miệng, kiểm tra 15 phút, kiểm tra 1 tiết, thi cuối kỳ (5/10/15/70). Mỗi 1 môn học xã hội có 5 đầu điểm: Điểm chuyên cần, điểm bài luận, kiểm tra 1 tiết, kiểm tra 2 tiết, thi cuối kỳ (5, 10, 10, 15, 60).

Hãy viết một chương trình vận dụng lập trình hướng đối tượng và tính kế thừa thực hiện các nhiệm vụ sau:

- Load dữ liệu bảng điểm chi tiết vào.

- Tính điểm tổng kết trung bình cho từng môn.

- Xếp loại học lực của học viên (trung bình, trung bình khá, khá, giỏi dựa vào điểm tổng kết trung bình của học viên).

- Đưa ra đánh giá sơ bộ về kết quả thi đại học dự kiến của học sinh thuộc loại nào (loại 1, loại 2, loại 3) theo các khối: A, A1, B, C, D dựa trên điểm tổng kết trung bình cho từng môn.

***

Hướng dẫn

Hãy viết 1 chương trình “tinhtoanbangdiem_python” có các class và phương thức sau:

a. Hãy viết 1 class “BANGDIEM” có các phương thức sau:

- Phương thức load_dulieu: Load dữ liệu từ đường dẫn file vào một list.

- Phương thức tinhdiem_trungbinh: Chức năng tương tự như hàm tinhdiem_trungbinh của assignment 2, input của phương thức tinhdiem_trungbinh thay thế đường dẫn bảng điểm chi tiết bằng output của phương thức load_dulieu.

- Phương thức luudiem_trungbinh: Chức năng tương tự như hàm luudiem_trungbinh của assignment 2.

b. Hãy viết 1 class “DANHGIA” có các phương thức sau:

- Kế thừa class “BANGDIEM” và tất cả các thuộc tính của nó.

- Phương thức xeploai_hocsinh: Chức năng tương tự như hàm xeploai_hocsinh của assignment 2. Input của phương thức xeploai_hocsinh thay thế đường dẫn bảng điểm trung bình bằng output của phương thức load_dulieu kế thừa từ class “BANGDIEM”.

- Phương thức xeploai_thidaihoc_hocsinh: Chức năng tương tự như hàm xeploai_thidaihoc_hocsinh của assignment 2. 

c. Hàm main:

Input: 

- Đường dẫn bảng điểm chi tiết cho từng môn của tất cả học sinh lưu trong file “diem_chitiet.txt”.

- Đường dẫn để lưu output.

Yêu cầu: Kết quả được lưu ra file “diem_trungbinh.txt” và “danhgia_hocsinh.txt” theo đường dẫn cho trước.

Chi tiết:

- Sử dụng 2 class “BANGDIEM” và “DANHGIA” để giải quyết bài toán bằng cách khai báo 1 đối tượng của class “DANHGIA” và chạy các phương thức cần thiết.

d. Yêu cầu nâng cao:

 Hãy tách phương thức xeploai_thidaihoc_hocsinh trong class DANHGIA thành 3 class:

- Class TUNHIEN: Phương thức xeploai_thidaihoc_hocsinh chạy cho khối tự nhiên (A, A1 và B).

- Class XAHOI: Phương thức xeploai_thidaihoc_hocsinh chạy cho khối xã hội (C).

- Class COBAN: Phương thức xeploai_thidaihoc_hocsinh chạy cho khối cơ bản (D).

- Các class này đều kế thừa class DANHGIA và các thuộc tính của nó.

Lưu ý: 

- Có thể vẫn giữ việc khai báo phương thức xeploai_thidaihoc_hocsinh ở class DANHGIA nếu học viên muốn sử dụng kỹ thuật overiding hoặc super.

- Nếu các bạn phát triển thêm phần advance, hàm main cần phải chỉnh sửa lại để kết quả cuối cùng của hàm main vẫn không thay đổi so với phương án làm theo yêu cầu cơ bản (đọc kỹ yêu cầu về output của hàm main).