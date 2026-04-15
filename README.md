[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23574059&assignment_repo_type=AssignmentRepo)
# Day 10 Lab: Data Pipeline & Data Observability

**Student Email:** email@example.com
**Name:** (Dien ten cua ban)

---

## Mo ta

Bài lab này yêu cầu xây dựng một pipeline ETL tự động để xử lý dữ liệu sản phẩm từ file JSON, kiểm tra và loại bỏ dữ liệu không hợp lệ, chuẩn hóa thông tin, tính giá sau giảm giá và lưu kết quả ra file CSV. Ngoài ra, em đã thực hiện so sánh kết quả của agent khi sử dụng dữ liệu sạch và dữ liệu lỗi, phân tích ảnh hưởng của chất lượng dữ liệu đến kết quả AI, và hoàn thành báo cáo theo yêu cầu.

---

## Cach chay (How to Run)

### Prerequisites
```bash
pip install pandas
```

### Chay ETL Pipeline
```bash
python solution.py
```

### Chay Agent Simulation (Stress Test)
```bash
# Mo ta cach ban chay thi nghiem Clean vs Garbage data
    Testing with CLEAN data:
    Agent: Based on my data, the best choice is Laptop at $1200.

    Testing with GARBAGE data:
    Agent: Based on my data, the best choice is Nuclear Reactor at $999999.

```

---

## Cau truc thu muc

```
├── solution.py              # ETL Pipeline script
├── processed_data.csv       # Output cua pipeline
├── experiment_report.md     # Bao cao thi nghiem
└── README.md                # File nay
```

---

## Ket qua

Tóm tắt kết quả:
- Tổng số records đầu vào: 5
- Số records hợp lệ sau khi validate: 3
- Số records bị loại bỏ: 2 (do giá <= 0 hoặc thiếu category)
- File processed_data.csv đã được tạo thành công với 3 records sạch, đầy đủ thông tin.
Kết quả chi tiết được ghi nhận trong quá trình chạy pipeline và có thể kiểm tra lại trong file processed_data.csv.
