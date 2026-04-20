# Deep Learning - Thực hành

Repository tổng hợp các notebook thực hành môn Deep Learning, trình bày rõ mục tiêu và nội dung của từng lab.

## Tổng quan các lab

### 1) `Lab1_Numpy_Pandas.ipynb`
**Mục tiêu:** Làm quen thao tác dữ liệu nền tảng bằng NumPy và Pandas.

**Nội dung đã thực hiện:**
- Kiểm tra điều kiện trên mảng (`all`, `any`)
- So sánh mảng bằng các hàm NumPy (`greater`, `less`, ...)
- Tạo các mảng/ma trận thường dùng (`zeros`, `ones`, `identity`, ma trận biên,...)
- Tính toán trên mảng nhiều chiều (tổng theo trục, inner product, broadcasting)
- Thao tác cơ bản với Pandas Series/DataFrame:
  - Cộng/trừ/nhân/chia giữa các Series
  - Chuyển cột DataFrame thành Series
  - Sắp xếp dữ liệu
  - Reindex và lọc phần tử khác biệt giữa 2 Series

**Kết quả đạt được:** Thành thạo cú pháp nền tảng để chuẩn bị cho các bài toán xử lý dữ liệu và học sâu.

---

### 2) `Lab1_Tensorflow.ipynb`
**Mục tiêu:** Làm quen TensorFlow từ tensor cơ bản đến xây dựng mô hình tính toán đơn giản.

**Nội dung đã thực hiện:**
- Tạo tensor với các cách khác nhau (`zeros`, `fill`, `range`)
- Sinh dữ liệu ngẫu nhiên (`random.normal`, `random.uniform`)
- Trộn dữ liệu (`shuffle`) và cắt ảnh/tensor (`random_crop`)
- Xử lý điều kiện trên tensor
- Thực hiện phép toán tensor (cộng, trừ, nhân, chia)
- Viết hàm/graph với `@tf.function`
- Xây dựng các module/model đơn giản:
  - Tính tổng 2 tensor
  - Tính hiệu/tích 2 tensor
  - Tính chu vi hình chữ nhật từ đầu vào `a`, `b`

**Kết quả đạt được:** Hiểu luồng xử lý tensor trong TensorFlow và cách tổ chức phép toán dưới dạng model.

---

### 3) `Data_Pre_Processing.ipynb`
**Mục tiêu:** Thực hành tiền xử lý dữ liệu thực tế trên bộ dữ liệu Titanic.

**Nội dung đã thực hiện:**
- Tách cột `Name` thành `firstName` và `secondName`, sau đó bỏ cột gốc
- Chuẩn hóa cột `Sex` (`male/female` → `M/F`)
- Thử áp dụng `map`/`pipe` để viết quy trình xử lý gọn hơn
- Xử lý thiếu dữ liệu cho `Age`:
  - Theo trung bình toàn bộ
  - Theo nhóm `Pclass` (so sánh cách làm)
- Tạo biến phân nhóm tuổi `Agegroup` (Kid/Teen/Adult/Older)
- Xử lý cột `Cabin`:
  - Điền thiếu bằng `Unknown`
  - Tách loại cabin theo ký tự đầu
- Phân tích và trực quan:
  - Tỉ lệ sống sót theo giới tính
  - Phân bố giới tính theo hạng vé (`Pclass`)
  - Xác suất sống sót theo thông tin người đi cùng
  - Sống sót/thiệt mạng theo `Pclass` và `Embarked`

**Kết quả đạt được:** Hoàn thiện pipeline tiền xử lý + trực quan dữ liệu cơ bản cho bài toán machine learning.

## Môi trường chạy

- Python 3.x
- Jupyter Notebook hoặc Google Colab
- Thư viện sử dụng:
  - `numpy`
  - `pandas`
  - `tensorflow`
  - `matplotlib`
  - `seaborn`

## Cách chạy nhanh

### Chạy local
```bash
git clone https://github.com/HoaiNam2k5/Deep_Learning_Practice.git
cd Deep_Learning_Practice
pip install numpy pandas tensorflow matplotlib seaborn notebook
jupyter notebook
```

Sau đó mở lần lượt các file:
- `Lab1_Numpy_Pandas.ipynb`
- `Lab1_Tensorflow.ipynb`
- `Data_Pre_Processing.ipynb`

### Chạy trên Google Colab
- Mở notebook bằng Colab badge trong từng file, hoặc upload trực tiếp file `.ipynb`.

## Cấu trúc hiện tại

```text
Deep_Learning_Practice/
├── Lab1_Numpy_Pandas.ipynb
├── Lab1_Tensorflow.ipynb
├── Data_Pre_Processing.ipynb
└── README.md
```
