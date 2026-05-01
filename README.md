# 🚀 DATATHON PROJECT

## 📌 Giới thiệu
Dự án này được thực hiện trong khuôn khổ **Datathon** – một cuộc thi phân tích dữ liệu nhằm giải quyết các bài toán thực tế thông qua dữ liệu.

Mục tiêu của dự án:
- Phân tích dữ liệu
- Xây dựng mô hình 
- Trực quan hóa kết quả
- Đưa ra insight / kết luận
## 🧠 Công nghệ sử dụng
- Tech Stack: Python (NumPy, Pandas, Matplotlib, Seaborn,Scikit-learn,…),Shap,Time Series Walk-forward CV.
- Jupyter Notebook / Google Colab.
- Machine Learning Algorithms: Random Forest, Gradient Boosting, XGBoost (XGBRegressor).
  
## 📂 Cấu trúc thư mục

```
DATATHON/
│── README.md
│── Datathon_P1.ipynb   # Code câu hỏi trắc nghiệm
│── Datathon_P2.ipynb   # Xử lý dữ liệu & insight 
│── Datathon_P3.ipynb   # Mô hình & đánh giá
```
## Hướng dẫn chạy Datathon_Task3 trên Google Colab

## 📂 Chuẩn bị dữ liệu

Đảm bảo Google Drive của bạn có cấu trúc như sau:
```
MyDrive/Datathon/
├── Analytical/
│ ├── sales.csv
│ └── sample_submission.csv
├── Transaction/
│ ├── returns.csv
│ └── reviews.csv
├── Operational/
│ ├── inventory.csv
│ └── web_traffic.csv
├── orders.csv
├── shipments.csv
└── master_features_giahuy.csv
```

---

## ▶️ Các bước chạy

### 🔹 Block 1: Training

- Mount Google Drive  
- Load toàn bộ dữ liệu  
- Tạo feature  
- Huấn luyện 3 mô hình:
  - Random Forest (seed = 42)
  - Gradient Boosting (seed = 42)
  - XGBoost (seed = 11)
- Sử dụng **Walk-forward Cross Validation**
- Kết quả **R² score** sẽ được in ra cho từng fold  

---

### 🔹 Block 2: Evaluation & Submission

- Tạo **SHAP plot** để giải thích mô hình  
- Xuất file `submission.csv` tại:
MyDrive/submission.csv.
Toàn bộ random seed đã được cố định (RF: 42, GBM: 42, XGBoost: 11). Không cần cài thêm thư viện ngoài môi trường mặc định của Colab.
