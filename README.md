# ptdl-project
# 📊 Phân tích xu hướng thị trường mỹ phẩm – Sephora

## 📌 Giới thiệu  
Dự án này khám phá xu hướng thị trường mỹ phẩm trên **Sephora** thông qua phân tích dữ liệu, trực quan hóa và phân tích cảm xúc khách hàng.  
Mục tiêu: nhận diện thương hiệu nổi bật, sản phẩm phổ biến, và xu hướng tiêu dùng.

---

## 🛠 Các bước thực hiện

### 1. Thu thập & Chuẩn bị dữ liệu
- Đọc dữ liệu từ file CSV.
- Kiểm tra kích thước, cấu trúc, kiểu dữ liệu và tên cột.

### 2. Tiền xử lý & Làm sạch dữ liệu
- Xử lý giá trị thiếu (*missing values*) bằng `pandas` và `missingno`.
- Chuẩn hóa dữ liệu văn bản và giá sản phẩm.

### 3. Phân tích dữ liệu (EDA)
- Xác định các thương hiệu chiếm thị phần lớn.
- Tìm thương hiệu & sản phẩm phổ biến.
- Đánh giá sản phẩm theo **value for money** (*value_price*).

### 4. Trực quan hóa dữ liệu
- Tạo biểu đồ cột, tròn, phân tán và biểu đồ động với `Matplotlib`, `Seaborn`, `Plotly Express`.

### 5. Phân tích cảm xúc (Sentiment Analysis)
- Sử dụng `TextBlob` phân loại đánh giá: tích cực, tiêu cực, trung tính.

### 6. Word Cloud
- Trích xuất từ khóa nổi bật trong đánh giá để nhận diện xu hướng.

---

## 🖼 Demo kết quả

### Top 10 thương hiệu phổ biến
![Top Brands](images/top_brands.png)

### Phân bố giá sản phẩm
![Price Distribution](images/price_distribution.png)

### Phân tích cảm xúc đánh giá khách hàng
![Sentiment Analysis](images/sentiment_analysis.png)

### Từ khóa nổi bật (Word Cloud)
![Word Cloud](images/wordcloud.png)

---

## 💻 Công nghệ sử dụng
- **Ngôn ngữ:** Python  
- **Thư viện:** Pandas, Numpy, Matplotlib, Seaborn, Plotly, Missingno, TextBlob, WordCloud  

---

## 🚀 Cách chạy dự án
```bash
# Clone repo
git clone https://github.com/trangnguyen-art/ptdl-project.git

# Cài đặt thư viện
pip install -r requirements.txt

# Mở notebook
jupyter notebook Phân_tích_xu_hướng_thị_trường_mỹ_phẩm.ipynb
