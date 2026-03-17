# Dự đoán lượng khí thải CO₂ dựa trên mức tiêu thụ năng lượng

## 1. Giới thiệu

Đề tài tập trung vào bài toán phân tích dữ liệu và đánh giá tính khả thi của việc xây dựng mô hình dự đoán lượng phát thải CO₂ hàng năm của một quốc gia dựa trên mức tiêu thụ năng lượng.

Dữ liệu được thu thập từ nguồn:
https://yearbook.enerdata.net/

Thông qua phương pháp:

- Web Scraping kết hợp API Extraction

Sau đó, dữ liệu được làm sạch, xử lý và phân tích nhằm trả lời các câu hỏi:

- Những yếu tố tiêu thụ năng lượng nào ảnh hưởng mạnh nhất đến lượng khí thải CO₂ của một quốc gia?
- Liệu có thể dự đoán lượng CO₂ dựa trên các yếu tố này hay không?

## 2. Mục tiêu

- Xây dựng bộ dữ liệu về tiêu thụ năng lượng và phát thải CO₂ có thể tái sử dụng cho phân tích và mô hình hóa.
- Làm sạch dữ liệu và chuẩn hóa các đặc trưng quan trọng nhằm giảm nhiễu và xử lý outliers.
- Trực quan hóa và phân tích mối quan hệ giữa các loại năng lượng và lượng phát thải CO₂
- Đánh giá mức độ ảnh hưởng của từng yếu tố năng lượng đến phát thải CO₂.

## 3. Cấu trúc thư mục

- _feature_engineering.ipynb_: Notebook phân tích dữ liệu, trực quan hóa và đưa ra kết luận
- _raw_data.jsonl_: Dữ liệu thô
- _clean_data_: Dữ liệu sạch cuối cùng phục vụ phân tích

## 4. Công nghệ sử dụng

Dự án sử dụng:

- Python 3.10+

Các thư viện chính:

- Selenium
- Requests
- urllib3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Statsmodels
- Scikit-learn
- Pycountry-convert
- Jupyter Notebook
- IPykernel

Môi trường chạy

- Jupyter Notebook

### 5. Yêu cầu môi trường

#### 5.1 Kiểm tra Python đã cài chưa

Chạy lệnh:
`python --version`
Nếu chưa có Python, cài từ trang chính thức: https://www.python.org/downloads/

### 5.2 Tạo môi trường ảo

Di chuyển đến thư mục dự án rồi chạy:
`python -m venv .venv`

Kích hoạt môi trường ảo:
`.venv\Scripts\Activate.ps1`

### 5.3 Cài đặt các thư viên cần thiết
`pip install -r requirement.txt`

# 6. Hướng dẫn chạy dự án

Có thể chạy toàn bộ notebook _feature_engineering.ipynb_ bằng Run All hoặc thực thi lần lượt từng cell từ trên xuống dưới; cả hai cách đều cho kết quả tương đương.

