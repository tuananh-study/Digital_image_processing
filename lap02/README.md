# Xử lý ảnh số - Lab 02

## Giới thiệu

Notebook này là phần tiếp theo trong bài học xử lý ảnh số, tập trung vào các kỹ thuật nâng cao như:

- Tìm hiểu và áp dụng các kỹ thuật biến đổi cường độ ảnh (intensity transformation)
- Tăng cường chất lượng ảnh bằng các phương pháp: biến đổi cường độ, cân bằng lược đồ xám, biến đổi gamma, logarit.
- Vẽ và phân tích histogram ảnh.

## Cấu trúc dự án

```
Lab02_207ct09941.ipynb
README.md
.gitignore
```

## Công nghệ sử dụng

- Python 3.x
- OpenCV (cv2)
- NumPy
- Matplotlib
- Jupyter Notebook

## Các thư viện sử dụng

- import cv2
- import numpy as np
- import matplotlib.pyplot as plt

## Các chức năng chính

- Biến đổi âm bản ảnh(Negative Image): Giúp làm nổi bật chi tiết ở vùng sáng hoặc tối
- Biến đổi logarit (Log transformation): Tăng cường chi tiết vùng tối.
- Biến đổi gamma(Gamma correction): Điều chỉnh độ sáng tổng thể ảnh
- Cân bằng lược đồ xám (Histogram Equalization): Giúp phân phối lại độ sáng đều hơn, tăng độ tương phản ảnh
- Vẽ biểu đồ histogram ảnh: history cho thấy phân bố độ sáng anhr.
- Kéo giãn độ tương phản (Contrast Stretching): Trải đều mức sáng trong ảnh từ đen đến trắng

## Hướng dẫn sử dụng

### 1. Cài đặt thư viện cần thiết

```bash
pip install opencv-python numpy matplotlib jupyter
```

### 2. Mở notebook

```bash
jupyter notebook Lab02_207ct09941.ipynb
```

Chạy từng ô để quan sát kết quả xử lý ảnh trực quan.

## Giấy phép

Dự án phục vụ mục đích học tập cá nhân.

## Tác giả

- MSSV: 207CT09941
- Họ tên: Phạm Tuấn Anh
