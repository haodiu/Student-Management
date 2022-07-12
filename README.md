# Student-score-management
Quản lý điểm sinh viên theo hệ tín chỉ
>Publication and Subcription:

  - Sever CNTT + VT: Horizontal Fragmentation 
  
  ![image](https://user-images.githubusercontent.com/67044416/178482290-71f5fb54-5eeb-4be9-b80e-8499a751d61e.png)
  ![image](https://user-images.githubusercontent.com/67044416/178482521-fdc8339a-dbfa-48c5-a7c2-32a51b3ef8d8.png)
  
  - Sever HOCPHI: Vertical Fragmentation
  
  ![image](https://user-images.githubusercontent.com/67044416/178482646-f5ba7427-0c65-4850-9310-09eb2433e9c8.png)
>Link Server:
  - Ở server1(CNTT) tạo LINK0 để kết nối từ server1 về server chủ
  - Ở server2(VT) tạo LINK0 để kết nối từ server2 về server chủ
  - Trên sever chủ ta tạo link server có tên LINK0 kết nối với chính nó để tránh phát sinh lỗi.
  Lưu ý: Điều kiện để kết nối bằng link server cần tên link server giống nhau ở 2 server cần kết nối.
>Authorization:
  - Nếu login thuộc nhóm PGV thì login đó có thể chọn bất kỳ khoa nào để toàn quyền làm việc bằng cách chọn tên khoa, và tìm dữ liệu trên phân mảnh tương ứng. Login nhóm này được tạo tài khoản cho nhóm PGV, Khoa.  
  - Nếu login thuộc nhóm Khoa thì ta chỉ cho phép toàn quyền làm việc trên khoa đã đăng nhập   và tìm dữ liệu trên phân mảnh tương ứng để in. Login này được tạo tài khoản cho nhóm Khoa.
  - Nhóm SV chỉ được đăng ký lớp tín chỉ. Tất cả sinh viên đều dùng chung 1 login đăng nhập.

  - Nếu login thuộc nhóm PKT thì chỉ được quyền cập nhật dữ liệu đóng học phí của sinh viên, chỉ được tạo tài khoản mới thuộc cùng nhóm.
  Chương trình cho phép ta tạo các login, password và cho login này làm việc với quyền hạn tương ứng. Căn cứ vào quyền này khi user login vào hệ thống, ta sẽ biết người đó được quyền làm việc với mảnh phân tán nào hay trên tất cả các phân mảnh.
  
**Đọc file De2-QLDSV_HTC-SQLSERVER_PhanTan.docx để biết chi tiết yêu cầu đề tài**
  
>Project sử dụng visual studio 2019 + devexpress 19.2.5
