Lab 5 – Xử lý ảnh số: Phân vùng, Gán nhãn và Dò tìm Đối tượng
📌 Mô tả tổng quan
Notebook này bao gồm chuỗi các bài thực hành về xử lý ảnh số, sử dụng Python và thư viện OpenCV, Scikit-image, nhằm thực hiện các kỹ thuật:

Phân vùng và gán nhãn các đối tượng trong ảnh nhị phân

Dò biên, xác định góc cạnh đối tượng

Phân tích hình dạng bằng Hough Transform

Phát hiện đường thẳng và đường tròn

Nội dung chi tiết

1. Gán nhãn cho các phân vùng ảnh (Image Labeling)
   Sử dụng ảnh nhị phân sau ngưỡng hóa (Otsu threshold)

Áp dụng thuật toán connected component labeling

Tính toán các thuộc tính vùng như: diện tích, trọng tâm (centroid), bounding box

Kết quả được trực quan hóa với matplotlib

2. Dò biên và phát hiện đặc trưng hình học
   2.1 Dò cạnh theo chiều dọc
   Tính sai khác giữa ảnh gốc và ảnh bị dịch 1 pixel để tìm cạnh

2.2 Dò cạnh bằng bộ lọc Sobel
Áp dụng Sobel filter theo cả 2 trục x và y để phát hiện biên

2.3 Phát hiện góc bằng Harris Corner Detection
Tự cài đặt hàm Harris() để xác định các góc trong ảnh

3. Phân tích hình dạng bằng Hough Transform
   3.1 Dò tìm đường thẳng
   (Phần này có thể nằm trong các cell tiếp theo chưa đọc hết)

3.2 Dò tìm đường tròn
Áp dụng Hough Circle Transform trên ảnh bird.png

Yêu cầu cài đặt
Cài đặt thư viện cần thiết:

```bash
pip install numpy opencv-python matplotlib pillow scikit-image imageio
```

## Tác giả

- MSSV: 207CT09941
- Họ tên: Pham Tuấn Anh
