# Association-Rule-Analysis
Market basket analysis using Apriori algorithm to suggest product combinations.

Phân Tích Luật Kết Hợp (Association Rule Analysis)

Dự án này thực hiện phân tích giỏ hàng (Market Basket Analysis) bằng thuật toán **Apriori** để khám phá các mối liên hệ giữa các sản phẩm thường được mua cùng nhau. Mục tiêu là giúp đưa ra các quyết định kinh doanh như gợi ý sản phẩm, bán kèm, khuyến mãi hiệu quả.

Notebook được viết bằng **Python** sử dụng thư viện `mlxtend`, `pandas` và `matplotlib`, thực hiện trên môi trường **Jupyter Notebook**.

## Mục Tiêu
- Phân tích tập dữ liệu giao dịch để tìm ra các **tập mặt hàng thường xuyên (frequent itemsets)**.
- Sinh ra các **luật kết hợp (association rules)** với các chỉ số như:
  - Support (độ hỗ trợ)
  - Confidence (độ tin cậy)
  - Lift (độ nâng)
- Từ đó đề xuất các **chiến lược gợi ý sản phẩm** cho khách hàng.
  
## Công Cụ & Thư Viện
- Python 3.x
- Jupyter Notebook
- `pandas`
- `mlxtend` (Apriori, association_rules)
- `matplotlib`, `seaborn` (trực quan hóa)

## Các Bước Thực Hiện
1. **Tiền xử lý dữ liệu**
   - Chuyển đổi dữ liệu sang dạng one-hot encoding để phù hợp với Apriori
2. **Áp dụng thuật toán Apriori**
   - Xác định các tập phổ biến dựa trên `min_support` (ngưỡng độ hỗ trợ)
3. **Sinh luật kết hợp**
   - Tính các luật thoả mãn `min_confidence` và `lift`
4. **Phân tích & lọc luật**
   - Tìm ra các luật có ý nghĩa để áp dụng thực tế
