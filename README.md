# Retail Customer Behavior Analysis: Unlocking High-Value Segments

**📌 Xem Báo cáo Hoàn chỉnh (Full HTML Report):** 
👉 [Bấm vào đây để xem toàn bộ phân tích và biểu đồ trực quan](link-xem-truc-tiep)

---

## 1. Mục tiêu Dự án 
Sử dụng dữ liệu hành vi mua sắm và phản hồi Marketing trong 2 năm để phân khúc khách hàng. Từ đó, xác định tệp khách hàng tiềm năng mang lại lợi nhuận và đề xuất chiến lược "Tiếp thị mục tiêu" (Targeted Marketing) thay vì chạy quảng cáo đại trà.

## 2. Công cụ Kỹ thuật 
* **Ngôn ngữ:** R
* **Thư viện xử lý dữ liệu:** `tidyverse`, `dplyr`, `lubridate`, `janitor`
* **Trực quan hóa:** `ggplot2`, `scales`
* **Đóng gói báo cáo:** RMarkdown (`.Rmd` -> `.html`)

## 3. Thành quả Cốt lõi 
* **Data Quality Assessment (DQA):** Xử lý các điểm khuyết thiếu (NULL Income) bằng phương pháp nội suy trung vị có điều kiện để bảo toàn tệp khách hàng giá trị cao.
* **Feature Engineering:** Xây dựng bộ biến mới (`Deal_Dependency`, `Behavior_Type`, `Family_Status`) để lượng hóa mức độ sử dụng khuyến mãi của khách hàng.
* **Actionable Insights:** Bóc tách hành vi tệp khách hàng *High Income - Organic Buyer* dù chỉ chiếm số lượng nhỏ nhưng có tỷ lệ phản hồi chiến dịch Marketing lên đến 41.6%.

---

Dự án này sử dụng bộ dữ liệu [Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis) được công bố bởi **Dr. Omar Romero - Hernandez** trên nền tảng Kaggle. 

Xin gửi lời cảm ơn trân trọng đến tác giả vì đã cung cấp một bộ dữ liệu mang tính thực tiễn, giúp tôi có cơ hội rèn luyện tư duy phân tích hành vi và áp dụng các kỹ năng xử lý dữ liệu vào một bài toán kinh doanh thực tế.
