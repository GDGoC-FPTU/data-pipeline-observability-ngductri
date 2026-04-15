# Experiment Report: Data Quality Impact on AI Agent

**Student ID:** AI20K-2A202600394
**Name:** Nguyễn Đức Trí
**Date:** 15/04/2026

---

## 1. Ket qua thi nghiem

Chay `agent_simulation.py` voi 2 bo du lieu va ghi lai ket qua:

| Scenario | Agent Response | Accuracy (1-10) | Notes |
|----------|----------------|-----------------|-------|
| Clean Data (`processed_data.csv`) | (Ghi cau tra loi cua Agent) | | |
| Garbage Data (`garbage_data.csv`) | (Ghi cau tra loi cua Agent) | | |

---

## 2. Phan tich & nhan xet

### Tai sao Agent tra loi sai khi dung Garbage Data?

Agent trả lời sai khi sử dụng Garbage Data là do dữ liệu đầu vào chứa nhiều vấn đề nghiêm trọng như: Duplicate IDs (trùng lặp khoá chính khiến agent nhầm lẫn giữa các sản phẩm), wrong data types (giá tiền bị ghi sai kiểu, ví dụ 'ten dollars' thay vì số, làm cho việc so sánh giá bị lỗi), outliers (giá trị bất thường như giá quá cao hoặc quá thấp khiến agent chọn sai sản phẩm tốt nhất), null values (dữ liệu thiếu thông tin quan trọng như category hoặc id). Những lỗi này làm cho quá trình xử lý, lọc và truy vấn dữ liệu của agent bị sai lệch, dẫn đến kết quả trả lời không chính xác hoặc không hợp lý. Điều này cho thấy chất lượng dữ liệu đầu vào ảnh hưởng trực tiếp đến hiệu quả và độ tin cậy của hệ thống AI, bất kể prompt có tốt đến đâu.

---

## 3. Ket luan

**Quality Data > Quality Prompt?** (Dong y hay khong? Giai thich ngan gon.)

Đồng ý. Dữ liệu chất lượng cao là nền tảng để AI đưa ra kết quả chính xác, dù prompt có tốt đến đâu nhưng dữ liệu sai lệch thì kết quả vẫn sẽ không đáng tin cậy. Prompt tốt chỉ phát huy hiệu quả khi dữ liệu đầu vào đã được làm sạch và chuẩn hóa.
