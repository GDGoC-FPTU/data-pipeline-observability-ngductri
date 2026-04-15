[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23574059&assignment_repo_type=AssignmentRepo)
# Day 10 Lab: Data Pipeline & Data Observability

**Student Email:** email@example.com
**Name:** (Dien ten cua ban)

---

## Mo ta

Pipeline thuc hien ETL tu file JSON, loai bo ban ghi khong hop le (gia <= 0, category rong), chuan hoa category dang Title Case, tinh discounted_price va them processed_at. Ket qua duoc luu ra CSV va dung de danh gia anh huong chat luong du lieu den agent.

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
python solution.py
python generate_garbage.py
python agent_simulation.py
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

Tu raw_data.json co 5 records, sau validate con 3 records hop le va 2 records bi loai (gia <= 0 hoac category rong). File processed_data.csv duoc tao voi cac cot: price, discounted_price, category (Title Case) va processed_at.
