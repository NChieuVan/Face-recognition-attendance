# Face-recognition-attendance
# FaceDatabase

`FaceDatabase` là một class Python dùng để quản lý cơ sở dữ liệu ảnh khuôn mặt, hỗ trợ các chức năng:

- Tạo và lưu dữ liệu ảnh khuôn mặt trong file JSON
- Thêm, sửa, xóa thông tin ảnh trong database
- Phát hiện khuôn mặt trong ảnh bằng mô hình YOLO
- So sánh và điểm danh khuôn mặt bằng thư viện DeepFace

---

## Tính năng chính

- **Khởi tạo** với file JSON lưu dữ liệu ảnh và model YOLO nhận diện khuôn mặt.
- **Cắt ảnh khuôn mặt** từ ảnh đầu vào dựa trên kết quả YOLO.
- **Lưu trữ ảnh** và metadata (id, tên, đường dẫn) vào file JSON.
- **Thêm/Sửa/Xóa** ảnh trong database dễ dàng qua ID.
- **Điểm danh khuôn mặt**: nhận diện và so sánh khuôn mặt với ảnh trong database, xác định người tương ứng dựa trên ngưỡng độ tương đồng.

---

## Cài đặt

```bash
pip install ultralytics opencv-python deepface
