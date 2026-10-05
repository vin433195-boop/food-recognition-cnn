# Food Recognition — CNN + L2 Regularization

Ứng dụng web nhận dạng 20 loại món ăn từ ảnh, hiển thị top-3 dự đoán và thông tin dinh dưỡng.

- Mô hình: CNN 3 tầng Conv2D + L2 Regularization + Dropout (TensorFlow/Keras), huấn luyện trên 20 lớp của Food-101
- Giao diện: Streamlit
- Độ chính xác trên tập test (5.000 ảnh): khoảng 40% — đây là mô hình CNN cơ bản, chưa dùng transfer learning

## Chạy trên máy

```bash
pip install -r requirements.txt
streamlit run app.py
```

Cần đặt cùng thư mục với `app.py`: `food_model.h5`, `class_names.json`, `Mapping_Calories.json`.

Muốn lưu lịch sử dự đoán ra file khi chạy cá nhân: đặt biến môi trường `PERSIST_HISTORY=1`.
