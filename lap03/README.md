# Xử lý ảnh số - Lab 03

# Phân tích và trích xuất đặc trưng ảnh

## Giới thiệu

Notebook này thuộc Lab 03 trong chuỗi bài học xử lý ảnh số, tập trung vào các kỹ thuật phân tích đặc trưng và phát hiện biên ảnh như Sobel, Prewitt, Laplacian, Canny,... Dự án giúp hiểu rõ các toán tử phát hiện biên và ứng dụng trong thị giác máy tính.

## Cấu trúc dự án

```
Lab3_207ct09941.ipynb
README.md
.gitignore

Bai_Tap_Tang_Cuong.ipynb
file image "exercise"
```

## Công nghệ sử dụng

- Python 3.x
- OpenCV (cv2)
- NumPy
- Matplotlib
- Jupyter Notebook

## Các chức năng chính

- Phát hiện biên bằng toán tử Sobel: dunfg để phát hiện biên theo hướng ngang và dọc.
- Phát hiện biên bằng Prewitt: Tương tự sobel nhưng đơn giản hơn, hiệu quả kém hơn trong môi trường nhiễu nặng.
- Toán tử Laplacian: Phát hiện cácc điểm thay đổi biên độ mạnh, gồm cả chiều ngang và dọc.
- Phát hiện biên Canny: phương pháp phát hiện biên hiện đại, chính xác và phổ biến nhất.

- chọn đối tượng trong bức ảnh
- Thay đổi kích thước ảnh (zoom)
- xoay ảnh bằng hàm rotate(image, góc xoay)
- Loại bỏ những pixel nhiễu bằng Dilation, Erosion
- để ánh xạ vị trí mới cho ảnh đầu vào dùng hàm map_coordinate

## Note Bài tập tăng cường

## Bai Tap 01:

- Tịnh tiến ảnh dùng scipy.ndimage.shift() để di chuyển ảnh theo tọa độ (dy, dx):
  Trục Y (dọc) là dòng (row) → di chuyển theo dy
  Trục X (ngang) là cột (column) → di chuyển theo dx

- Tạo hiệu ứng sóng bằng biến đổi tọa độ (coordinate transformation):
  Dùng numpy.meshgrid() để tạo lưới tọa độ gốc.
  Dùng np.sin() để tạo lệch sóng tuần hoàn.
  Dùng scipy.ndimage.map_coordinates() để lấy mẫu lại ảnh theo tọa độ mới.

- Nội suy bậc 1 (bilinear interpolation):
  Khi biến đổi tọa độ, dùng order=1 để đảm bảo ảnh mượt mà, tránh răng cưa.

## Hướng dẫn sử dụng

### 1. Cài đặt thư viện cần thiết

```bash
pip install opencv-python numpy matplotlib jupyter
```

### 2. Mở notebook

```bash
jupyter notebook Lab3_207ct09941.ipynb
```

Chạy lần lượt các ô để quan sát kết quả phát hiện biên ảnh trực quan.

## Giấy phép

Dự án phục vụ mục đích học tập cá nhân.

## Tác giả

- MSSV: 207CT09941
- Họ tên: Pham Tuấn Anh
