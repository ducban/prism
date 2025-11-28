---
# Core Metadata
title: "Product Metrics Reference"
title_vi: "Bảng Tham Chiếu Chỉ Số Sản Phẩm"
framework_type: "Metrics"
category: ["Product Management", "Metrics", "Analytics", "KPIs"]

# Origin & Authority
author: "Various (Industry Standards)"
organization: "Product Management"
year_developed: "2000s"
original_source: "Product Management Best Practices"

# Root Integration
root_phase: ["Phase 5: Track Progress", "Phase 6: Launch & Release"]
root_commands: ["/phase5:metrics", "/phase6:analytics"]
when_to_use: "When defining success metrics, or tracking product performance"

# Difficulty & Time
complexity: "Low"
estimated_time: "Reference guide"
skill_level: "Beginner"

# Classification
tags: ["metrics", "kpis", "analytics", "measurement", "success-metrics", "reference"]
related_frameworks: ["AARRR", "North Star Metric", "OKRs"]
conflicts_with: []

# Metadata
version: "1.0"
last_updated: "2025-11-20"
language: "bilingual"
status: "Active"

# Learning Resources
external_resources:
  - type: "Article"
    title: "Product Metrics Guide"
    url: "https://www.productplan.com/glossary/product-metrics/"
    author: "ProductPlan"
    year: "2024"
  - type: "Tool"
    title: "Metrics Dashboard Template"
    url: "https://amplitude.com/blog/product-metrics"
    author: "Amplitude"
    year: "2024"
  - type: "Book"
    title: "Lean Analytics"
    url: "https://leananalyticsbook.com/"
    author: "Alistair Croll & Benjamin Yoskovitz"
    year: "2013"
---

## **Important Metrics Table / Bảng các chỉ số quan trọng**

| Metric (Chỉ số)                     | What it Measures (Đo lường điều gì)                               | Why it's Important (Tại sao lại quan trọng)                                          | Simple Formula (Công thức đơn giản)                      |     |
| :---------------------------------- | :---------------------------------------------------------------- | :----------------------------------------------------------------------------------- | :------------------------------------------------------- | --- |
| **GMV** (Gross Merchandise Value)   | Total transaction volume; the "headline" sales number.            | Shows scale, market share, and platform activity. Good for gauging growth potential. | `Price × Quantity` of all items sold.                    |     |
| **Revenue** (Doanh thu)             | The actual money earned from sales after deductions.              | The "top line." Shows the real income from core business operations.                 | `GMV - Returns - Discounts - Fees`                       |     |
| **Gross Profit** (Lợi nhuận gộp)    | Profitability of the products themselves, before operating costs. | Indicates if your pricing and production costs are sustainable.                      | `Revenue - Cost of Goods Sold (COGS)`                    |     |
| **Net Profit** (Lợi nhuận ròng)     | The final profit after all expenses are paid.                     | The "bottom line." The ultimate measure of financial health and sustainability.      | `Revenue - All Expenses (Operating, Interest, Taxes)`    |     |
| **AOV** (Average Order Value)       | The average amount a customer spends per transaction.             | Helps strategize upselling, cross-selling, and marketing campaigns.                  | `Total Revenue / Number of Orders`                       |     |
| **CAC** (Customer Acquisition Cost) | The cost to acquire one new customer.                             | Measures marketing and sales efficiency. Crucial for growth models.                  | `Total Marketing & Sales Cost / Number of New Customers` |     |
| **LTV** (Lifetime Value)            | The total revenue a business can expect from a single customer.   | Determines long-term profitability. A healthy business has `LTV > CAC`.              | `Average Revenue per Customer × Customer Lifespan`       |     |
| **Cash Flow** (Dòng tiền)           | The net amount of cash moving in and out of the business.         | Shows liquidity and ability to pay bills. "Profit is an opinion, cash is a fact."    | `Total Cash Inflows - Total Cash Outflows`               |     |

---

## **Terminology Explained / Giải thích thuật ngữ**

Here are the core terms explained in professional and simple terms.

---

### **1. GMV (Gross Merchandise Value) / Tổng giá trị hàng hóa**

|                             | English                                                                                                                                                                                                                                      | Tiếng Việt                                                                                                                                                                                                                                                            |
| :-------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Professional Definition** | The total value of merchandise sold over a given period without any deductions for returns, allowances, or discounts. It represents the total sales volume on a platform or within a company.                                                | Tổng giá trị tiền tệ của tất cả hàng hóa được bán ra trong một kỳ nhất định, chưa trừ bất kỳ khoản chi phí nào như hàng trả lại, giảm giá, hay chiết khấu. Nó thể hiện tổng khối lượng bán hàng.                                                                      |
| **Layman's Terms**          | Think of GMV as the total price tag of everything in everyone's shopping cart as they check out. It's the "big, impressive number" that shows how much stuff is being sold, but it doesn't tell you how much money the store actually keeps. | Hãy tưởng tượng GMV là tổng giá trị ghi trên tất cả các hóa đơn tại một siêu thị trong một ngày. Nó là con số "hoành tráng" cho thấy siêu thị đó bận rộn và bán được nhiều hàng, nhưng không cho biết siêu siêu thị thực sự kiếm được bao nhiêu tiền.                 |
| **Real-World Example**      | A marketplace like Shopee or Amazon reports its GMV for a holiday sale. If a seller on the site sells 10 phones at $500 each and 20 cases at $25 each, their GMV is (10 × $500) + (20 × $25) = $5,000 + $500 = **$5,500**.                   | Một sàn TMĐT như Shopee báo cáo GMV trong đợt sale 11/11. Một người bán trên sàn đó bán được 10 điện thoại giá 5 triệu VNĐ/chiếc và 20 ốp lưng giá 250.000 VNĐ/chiếc. GMV của họ là: (10 × 5.000.000) + (20 × 250.000) = 50.000.000 + 5.000.000 = **55.000.000 VNĐ**. |

---

### **2. Revenue (Doanh thu)**

| | English | Tiếng Việt |
| :--- | :--- | :--- |
| **Professional Definition** | The income generated from normal business operations, calculated as the total sales of goods and services minus the cost of returns, allowances, and discounts. It is often referred to as the "top line" on an income statement. | Là thu nhập tạo ra từ hoạt động kinh doanh bình thường, được tính bằng tổng doanh số bán hàng và dịch vụ sau khi đã trừ đi chi phí hàng trả lại, các khoản giảm trừ và chiết khấu. Nó thường được gọi là "con số ở đầu" trên báo cáo kết quả kinh doanh. |
| **Layman's Terms** | This is the money that actually makes it into the cash register. From the big GMV number, you subtract the items customers returned, the discounts you gave them, and the fees you paid to the shopping mall (or platform like Amazon). This is your real take from selling stuff. | Đây là số tiền thực sự "về túi" bạn. Từ con số GMV hoành tráng, bạn trừ đi những món hàng khách trả lại, các khoản giảm giá bạn đã cho, và phí phải trả cho "chủ mặt bằng" (sàn TMĐT). Đây là số tiền bạn thực sự thu được từ việc bán hàng. |
| **Real-World Example** | Using the previous example: The seller's GMV was $5,500. One customer returned a phone ($500). The seller also offered a 10% site-wide discount and paid the marketplace a 15% commission fee on the final sale price. <br> Revenue = ($5,500 - $500) × 90% (discount) × 85% (commission) = $5,000 × 0.9 × 0.85 = **$3,825**. | Dựa trên ví dụ trên: GMV của người bán là 55.000.000 VNĐ. Một khách trả lại 1 điện thoại (5.000.000 VNĐ). Người bán cũng áp dụng giảm giá 10% trên toàn sàn và trả cho sàn 15% phí hoa hồng trên giá trị sau giảm. <br> Doanh thu = (55.000.000 - 5.000.000) × 90% (giảm giá) × 85% (phí sàn) = 50.000.000 × 0,9 × 0,85 = **38.250.000 VNĐ**. |

---

### **3. Net Profit (Lợi nhuận ròng)**

| | English | Tiếng Việt |
| :--- | :--- | :--- |
| **Professional Definition** | The actual profit of a business after all expenses, including operating costs (salaries, rent, marketing), interest, and taxes, have been deducted from revenue. It is known as the "bottom line." | Là lợi nhuận thực tế của một doanh nghiệp sau khi đã trừ đi tất cả các chi phí, bao gồm chi phí vận hành (lương, thuê mặt bằng, marketing), lãi vay, và thuế từ doanh thu. Nó được biết đến là "con số cuối cùng". |
| **Layman's Terms** | This is the money you get to keep and take home at the end of the day. You start with your Revenue, then pay for the products you sold (cost of goods), pay your employees' salaries, pay for rent and advertising, and finally pay the government (taxes). Whatever is left is your true profit. | Đây là số tiền bạn thực sự "lãi" được và có thể bỏ vào túi. Bạn bắt đầu với Doanh thu, rồi trả tiền cho hàng hóa bạn đã bán (giá vốn), trả lương nhân viên, tiền thuê nhà, quảng cáo, và cuối cùng là trả tiền cho nhà nước (thuế). Số tiền còn lại cuối cùng chính là lợi nhuận thực sự của bạn. |
| **Real-World Example** | The seller's Revenue was $3,825. The cost to buy the phones and cases (COGS) was $2,000. Other expenses (salary, ads, rent) totaled $1,000. Taxes were $150. <br> Net Profit = $3,825 (Revenue) - $2,000 (COGS) - $1,000 (Expenses) - $150 (Tax) = **$675**. | Doanh thu của người bán là 38.250.000 VNĐ. Chi phí nhập điện thoại và ốp lưng (giá vốn) là 20.000.000 VNĐ. Các chi phí khác (lương, quảng cáo, thuê mặt bằng) là 10.000.000 VNĐ. Thuế là 1.500.000 VNĐ. <br> Lợi nhuận ròng = 38.250.000 (Doanh thu) - 20.000.000 (Giá vốn) - 10.000.000 (Chi phí) - 1.500.000 (Thuế) = **6.750.000 VNĐ**. |

---

## Phân biệt GMV, Doanh thu và Lợi nhuận ròng

Hãy tưởng tượng bạn có một cửa hàng trên sàn thương mại điện tử (ví dụ: Shopee, Tiki).

### 1. GMV (Gross Merchandise Value) - Tổng giá trị hàng hóa

*   **Định nghĩa:** GMV là **tổng giá trị tiền tệ** của tất cả các sản phẩm được bán ra trong một khoảng thời gian nhất định, **chưa trừ bất kỳ khoản chi phí nào** như giảm giá, phí trả hàng, hay phí vận chuyển.
*   **Cách hiểu đơn giản:** GMV giống như "nhãn giá tổng hợp". Nó cho biết quy mô và "sức nóng" của giao dịch trên nền tảng/sàn.
    *   *Ví dụ:* Trong một ngày, cửa hàng của bạn bán được:
        *   10 chiếc áo giá 200.000 VNĐ/chiếc.
        *   5 chiếc quần giá 300.000 VNĐ/chiếc.
    *   => **GMV** của bạn trong ngày đó là: (10 * 200.000) + (5 * 300.000) = 2.000.000 + 1.500.000 = **3.500.000 VNĐ**.
*   **Bản chất:** GMV là chỉ số thể hiện **quy mô, thị phần và mức độ hoạt động** của một doanh nghiệp hoặc một sàn TMĐT. Nó rất quan trọng với các nhà đầu tư ở giai đoạn đầu để đánh giá tiềm năng tăng trưởng. Tuy nhiên, GMV cao không có nghĩa là công ty đang kiếm được nhiều tiền.

### 2. Doanh thu (Revenue) - Tiền thực tế thu về

*   **Định nghĩa:** Doanh thu là số tiền mà công ty **thực sự nhận được** sau khi đã trừ đi các khoản khấu trừ như hàng bị trả lại, giảm giá, chiết khấu, và các khoản phí phải chia sẻ cho đối tác (như phí hoa hồng cho sàn TMĐT).
*   **Cách hiểu đơn giản:** Đây là số tiền "về túi" thực tế của bạn từ việc bán hàng.
    *   *Tiếp theo ví dụ trên:* Trong số 3.500.000 VNĐ GMV, có:
        *   1 khách trả lại 1 chiếc áo (giá 200.000 VNĐ).
        *   Bạn chạy chương trình giảm giá 10% trên tổng hóa đơn.
        *   Sàn TMĐT thu phí hoa hồng 5% trên giá trị bán sau giảm giá.
    *   => **Doanh thu** của bạn sẽ được tính như sau:
        1.  GMV ban đầu: 3.500.000 VNĐ
        2.  Trừ hàng trả lại: 3.500.000 - 200.000 = 3.300.000 VNĐ
        3.  Trừ giảm giá (10%): 3.300.000 * 10% = 330.000 VNĐ. Giá trị sau giảm giá: 2.970.000 VNĐ.
        4.  Trừ phí sàn (5% trên 2.970.000): 2.970.000 * 5% = 148.500 VNĐ.
        5.  => **Doanh thu thực tế** = 2.970.000 - 148.500 = **2.821.500 VNĐ**.
*   **Bản chất:** Doanh thu (còn gọi là "top line") phản ánh **hiệu quả bán hàng** và là con số chính thức xuất hiện trên báo cáo kết quả kinh doanh. Nó cho thấy công ty đang tạo ra bao nhiêu tiền từ hoạt động cốt lõi.

### 3. Lợi nhuận ròng (Net Profit) - Tiền lãi cuối cùng

*   **Định nghĩa:** Đây là số tiền **còn lại cuối cùng** sau khi đã trừ **tất cả mọi chi phí** từ doanh thu, bao gồm: giá vốn hàng bán, chi phí vận hành (lương nhân viên, thuê mặt bằng, marketing), chi phí tài chính (lãi vay), và thuế.
*   **Cách hiểu đơn giản:** Đây là số tiền bạn thực sự "lãi" được và có thể bỏ vào túi sau khi đã trả hết mọi thứ.
    *   *Tiếp theo ví dụ trên:* Từ doanh thu 2.821.500 VNĐ, bạn phải chịu các chi phí:
        *   Giá vốn nhập hàng (10 áo + 5 quần): 1.500.000 VNĐ.
        *   Chi phí marketing quảng cáo: 300.000 VNĐ.
        *   Chi phí đóng gói, vận chuyển (phần bạn chịu): 100.000 VNĐ.
        *   Thuế TNDN (giả sử 20% trên lợi nhuận trước thuế).
    *   => **Lợi nhuận ròng** được tính như sau:
        1.  Doanh thu: 2.821.500 VNĐ
        2.  Trừ giá vốn: 2.821.500 - 1.500.000 = 1.321.500 VNĐ (Đây là Lợi nhuận gộp).
        3.  Trừ chi phí vận hành (marketing, đóng gói): 1.321.500 - 300.000 - 100.000 = 921.500 VNĐ (Đây là Lợi nhuận trước thuế).
        4.  Trừ thuế (20%): 921.500 * 20% = 184.300 VNĐ.
        5.  => **Lợi nhuận ròng** = 921.500 - 184.300 = **737.200 VNĐ**.
*   **Bản chất:** Lợi nhuận ròng (còn gọi là "bottom line") là thước đo **sự bền vững và khả năng sinh lời** của doanh nghiệp. Một công ty có thể có doanh thu rất cao nhưng nếu lợi nhuận ròng âm thì vẫn đang bị thua lỗ.

## Bảng tóm tắt so sánh

| Tiêu chí | GMV (Tổng giá trị hàng hóa) | Doanh thu (Revenue) | Lợi nhuận ròng (Net Profit) |
| :--- | :--- | :--- | :--- |
| **Bản chất** | Tổng giá trị giao dịch, chưa trừ chi phí | Số tiền thực tế thu về | Số tiền lãi cuối cùng |
| **Mức độ** | Quan sát ở cấp độ cao nhất, tổng thể | Phản ánh hiệu quả bán hàng | Phản ánh khả năng sinh lời bền vững |
| **Công thức** | Σ(Giá bán × Số lượng) | GMV - Giảm giá - Hàng trả lại - Phí sàn... | Doanh thu - Giá vốn - Tất cả chi phí - Thuế |
| **Ý nghĩa chính** | Thể hiện quy mô, thị phần, độ phủ | Thể hiện sức khỏe của hoạt động kinh doanh cốt lõi | Thể hiện hiệu quả quản lý và sự thành công về mặt tài chính |
| **Ai quan tâm?** | Nhà đầu tư giai đoạn đầu, đối tác, sàn TMĐT | Ban lãnh đạo, nhà đầu tư, cơ quan thuế | Chủ sở hữu, CEO, nhà đầu tư, ngân hàng |

---

## Các chỉ số quan trọng khác cần quan tâm

Ngoài 3 chỉ số trên, để có một bức tranh toàn cảnh, bạn cần xem xét thêm các metrics sau, tùy thuộc vào mô hình kinh doanh và giai đoạn phát triển:

### 1. Các chỉ số liên quan đến Lợi nhuận:
*   **Lợi nhuận gộp (Gross Profit):** `Doanh thu - Giá vốn hàng bán`. Cho thấy bạn lãi bao nhiêu trên mỗi sản phẩm bán ra, trước khi tính các chi phí vận hành khác.
*   **EBITDA (Earnings Before Interest, Taxes, Depreciation, and Amortization):** Lợi nhuận trước lãi vay, thuế và khấu hao. Thường được dùng để so sánh hiệu quả hoạt động giữa các công ty.

### 2. Các chỉ số liên quan đến Hoạt động & Khách hàng (quan trọng với TMĐT, SaaS):
*   **Giá trị đơn hàng trung bình (AOV - Average Order Value):** `Tổng doanh thu / Tổng số đơn hàng`. Giúp bạn hiểu khách hàng chi bao nhiêu tiền cho mỗi lần mua sắm.
*   **Chi phí thu hút khách hàng (CAC - Customer Acquisition Cost):** `Tổng chi phí Marketing & Bán hàng / Số khách hàng mới`. Cho biết bạn phải bỏ ra bao nhiêu tiền để có một khách hàng mới.
*   **Giá trị vòng đời khách hàng (LTV - Lifetime Value):** Tổng doanh thu dự kiến mà một khách hàng sẽ mang lại trong suốt thời gian họ gắn bó với bạn. Lý tưởng là `LTV > CAC`.
*   **Tỷ lệ khách hàng rời bỏ (Churn Rate):** Tỷ lệ phần trăm khách hàng ngừng sử dụng sản phẩm/dịch vụ của bạn trong một kỳ. Rất quan trọng với các mô hình đăng ký (subscription).

### 3. Các chỉ số liên quan đến Sức khỏe tài chính:
*   **Dòng tiền (Cash Flow):** Lượng tiền thực tế ra vào công ty. Một công ty có thể có lợi nhuận nhưng cạn kiệt dòng tiền và phá sản. "Lợi nhuận là quan điểm, dòng tiền là sự thật".
*   **Tỷ lệ đốt tiền (Burn Rate):** Tốc độ mà một startup (thường chưa có lợi nhuận) đang sử dụng hết tiền mặt của mình. Quan trọng để biết công ty còn tồn tại được bao lâu mà không cần thêm vốn.

### Kết luận

*   **GMV** cho thấy bạn **lớn đến mức nào**.
*   **Doanh thu** cho thấy bạn **bán hàng hiệu quả ra sao**.
*   **Lợi nhuận ròng** cho thấy bạn **kiếm được bao nhiêu tiền** và có **bền vững hay không**.

Việc hiểu rõ và theo dõi đồng bộ các chỉ số này sẽ giúp bạn có một cái nhìn toàn diện và chính xác, từ đó đưa ra những quyết định kinh doanh đúng đắn. Hy vọng giải thích này hữu ích cho bạn
---

## Keywords for Further Research

<!-- TODO: Add 5-7 keywords/concepts from this framework for user self-research -->
- [Framework-specific keyword 1]
- [Framework-specific keyword 2]
- [Framework-specific keyword 3]
