# AIO
Các thay đổi trước #Predict:

1. Sửa phần khai báo đường dẫn.
2. Sửa thứ tự tên lớp từ ['bào ngư xám + trắng', 'linh chi trắng','nấm mỡ','Đùi gà Baby (cắt ngắn)'] thành ['nấm mỡ', 'bào ngư xám + trắng', 'Đùi gà Baby (cắt ngắn)', 'linh chi trắng'] cho đúng với type index của submission mẫu
3. Sửa lại hàm preprocessing:
   - Cuối dòng khai báo transform có dấu phẩy gây lỗi ==> bỏ dấu phẩy chỗ cuối dòng khởi tạo transform
4. Sửa lại hàm transfer_learning:
  - Trong hàm transfer_learning khai báo data_loader nhưng lại dùng train_loader ==> chuyển train_loader trong thành data_loader
  - Thiếu phần khởi tạo writer ==> thêm phần khởi tạo writer và thêm 'writer.close()'
