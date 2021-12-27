HƯỚNG DẪN PHÂN CHIA TẬP DỮ LIỆU, XÂY DỰNG VÀ KIỂM TRA MÔ HÌNH ViT VÀ VGG16
Tất cả code đều được thực thi trên GG Colab.
---------------------------***************--------------------------------
1) Phân chia tập dữ liệu
- Chuẩn bị một tập dữ liệu và đặt vào cùng 1 thư mục rồi tải lên GG Drive.
- Mở file split_dataset.ipynb. 
- Đưa đường dẫn của thư mục dataset vào phần input ở cell code thứ 3.
- Tạo một thư mục ở GG Drive để chứa dataset được phân chia.
- Đưa dường dẫn thư mục vừa tạo vào phần output của cell code thứ 3.
- Thực thi tất cả các cell code.
---------------------------***************--------------------------------
2) Xây dựng mô hình ViT
- Tạo một thư mục ở GG Drive để lưu lại mô hình và các chỉ số trong quá trình huấn luyện.
- Tạo các file accuracy.txt, loss.txt, f1.txt, val_accuracy.txt, val_loss.txt, val_f1.txt, 
training_time.txt (chứa số 0), sau đó upload tất cả lên thư mục vừa tạo.
- Mở file train_ViT_model.ipynb.
- Đưa đường dẫn thư mục vừa tạo vào phần root_folder.
- Điều chỉnh các thông số batch_size, lr, max_epochs, max_patience_scheduler, max_patience_epoch tuỳ ý.
- Đưa đường dẫn tập train và tập validation của tập dữ liệu đã được phân chia vào train_dataset và val_dataset.
- Thực thi tất cả các cell code.
---------------------------***************--------------------------------
3) Xây dựng mô hình VGG16
- Tạo một thư mục ở GG Drive để lưu lại mô hình và các chỉ số trong quá trình huấn luyện.
- Tạo file training_time.txt (chứa số 0) và upload lên thư mục vừa tạo.
- Mở file train_vgg16_model.ipynb.
- Đưa đường dẫn thư mục vừa tạo vào pần root_folder.
- Khởi tạo các thông số INIT_LR, EPOCHS tuỳ ý.
- Đưa đường dẫn của tập train và tập val vào phần load_data.
- Thực thi tất cả các cell code.
---------------------------***************--------------------------------
4) Kiểm tra mô hinh ViT
- Chuẩn bị một thư mục temp chứa số lượng ảnh tuỳ ý để mô hình đự đoán và upload thư mục này lên GG Drive.
- Mở file test_ViT_model.ipynb.
- Đưa đường dẫn thư mục chứa mô hình cần kiểm tra vào root_folder.
- Đưa đường dẫn tập test vào test_dataset.
- Đưa đường dẫn thư mục temp vao sorted_dir và src.
- Thực thi tất cả các cell code.
----------------------------*************---------------------------------
5) Kiểm tra mô hình VGG16
- Chuẩn bị một thư mục temp chứa số lượng ảnh tuỳ ý để mô hình đự đoán và upload thư mục này lên GG Drive.
- Mở file test_vgg16_model.ipynb.
- Đưa đường dẫn thư mục chứa mô hình cần kiểm tra vào root_folder.
- Đưa đường dẫn tập test vào lúc gọi hàm load_data.
- Đưa đường dẫn thư mục temp vao sorted_dir và src.
- Thực thi tất cả các cell code.
------------------------------HẾT-----------------------------------------

