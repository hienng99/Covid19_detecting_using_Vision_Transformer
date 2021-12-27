INSTRUCTIONS FOR DATA SPLITTINGS, BUILDING AND TESTING ViT AND VGG16 MODELS
All code is executed on GG Colab.
------------------------------------------------------------------------------------------- ---------------
1) Split data set
- Prepare a dataset and put it in the same folder and then upload it to GG Drive.
- Open file split_dataset.ipynb.
- Put the path of the dataset folder into the input in cell code 3.
- Create a folder in GG Drive to store the partitioned dataset.
- Put the newly created directory path in the output of the 3rd cell code.
- Execute all cell code.
------------------------------------------------------------------------------------------- ---------------
2) Build ViT . model
- Create a folder in GG Drive to save models and metrics during training.
- Create files accuracy.txt, loss.txt, f1.txt, val_accuracy.txt, val_loss.txt, val_f1.txt,
training_time.txt (containing the number 0), then upload all to the folder just created.
- Open the file train_ViT_model.ipynb.
- Put the path of the newly created folder in the root_folder section.
- Adjust parameters batch_size, lr, max_epochs, max_patience_scheduler, max_patience_epoch as you like.
- Put the train set path and validation set of the split dataset into train_dataset and val_dataset.
- Execute all cell code.
------------------------------------------------------------------------------------------- ---------------
3) Build the VGG16 . model
- Create a folder in GG Drive to save models and metrics during training.
- Create a file training_time.txt (containing the number 0) and upload it to the newly created folder.
- Open the file train_vgg16_model.ipynb.
- Put the newly created folder path in the root_folder section.
- Initialize parameters INIT_LR, EPOCHS arbitrary.
- Put the path of the train set and the val file into the load_data section.
- Execute all cell code.
------------------------------------------------------------------------------------------- ---------------
4) Check the ViT . model
- Prepare a temp folder containing an arbitrary number of images for the model to predict and upload this folder to GG Drive.
- Open file test_ViT_model.ipynb.
- Put the directory path containing the model to be tested into the root_folder.
- Put the test file path into test_dataset.
- Put the temp directory path in sorted_dir and src.
- Execute all cell code.
-------------------------------------------------------------------------------------------- ---------------
5) Check model VGG16
- Prepare a temp folder containing an arbitrary number of images for the model to predict and upload this folder to GG Drive.
- Open file test_vgg16_model.ipynb.
- Put the directory path containing the model to be tested into the root_folder.
- Enter the test file path at the time of calling load_data function.
- Put temp directory path in sorted_dir and src.
- Execute all cell code.
------------------------------OVER------------------- ----------------------










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


