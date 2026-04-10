# Exploring-Mental-Health
# Khám Phá Dữ Liệu Sức Khỏe Tâm Thần — Exploring Mental Health Data

Dự án này tập trung vào việc phân tích và xây dựng mô hình máy học để dự đoán tình trạng trầm cảm dựa trên dữ liệu khảo sát sức khỏe tâm thần. Đây là một bài toán phân loại nhị phân sử dụng các thuật toán mạnh mẽ như CatBoost và LightGBM.

## 📋 Tổng quan dự án
- **Mục tiêu**: Dự đoán liệu một người có bị trầm cảm hay không (`Depression = 1`) dựa trên các yếu tố nhân khẩu học, áp lực và thói quen sinh hoạt.
- **Tập dữ liệu**: Gồm hơn 140,700 mẫu dữ liệu với 20 cột đặc trưng.
- **Công nghệ sử dụng**: Python, Pandas, Scikit-learn, CatBoost, LightGBM.

## 🛠️ Quy trình thực hiện
1. **Khám phá dữ liệu (EDA)**:
    - Phân tích và xử lý giá trị thiếu (hơn 80% thiếu ở các cột liên quan đến sinh viên/người đi làm).
    - Làm sạch nhiễu trong các cột như `Sleep Duration` và `Dietary Habits`.
2. **Feature Engineering**:
    - Tạo các đặc trưng mới như `Work_Sleep_Ratio` (tỷ lệ làm việc/ngủ), `Total_Pressure` (tổng áp lực) và `Total_Satisfaction`.
3. **Huấn luyện mô hình**:
    - Triển khai **CatBoostClassifier** làm mô hình chính.
    - So sánh với **LightGBM** và **Random Forest**.
4. **Đánh giá**:
    - Sử dụng các chỉ số: Accuracy, F1-score, và biểu đồ ma trận nhầm lẫn (Confusion Matrix).
    - Tối ưu hóa ngưỡng dự đoán (Threshold) để cân bằng giữa Precision và Recall.

## 🚀 Kết quả đạt được
- Mô hình đạt được độ chính xác và chỉ số F1-score ổn định trên tập kiểm tra.
- Các yếu tố như áp lực công việc/học tập và sự hài lòng trong cuộc sống là những đặc trưng quan trọng nhất để dự đoán trầm cảm.

## 💻 Hướng dẫn chạy code
1. Clone repository này:
   ```bash
   git clone [https://github.com/vdthcmus123/Exploring-Mental-Health.git](https://github.com/vdthcmus123/Exploring-Mental-Health.git)