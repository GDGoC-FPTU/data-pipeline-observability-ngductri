[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23574059&assignment_repo_type=AssignmentRepo)
# Day 10 Lab: Data Pipeline & Data Observability

**Student Email:** email@example.com  
**Name:** (Dien ten cua ban)

---

## Mo ta
ETL pipeline doc du lieu tu `raw_data.json`, loai bo record khong hop le (price <= 0 hoac category rong), chuan hoa du lieu (category Title Case, them `discounted_price` giam 10%), va them `processed_at` de theo doi thoi diem xu ly. Ket qua duoc ghi ra `processed_data.csv` va co log so record giu/loai.

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
python generate_garbage.py
python agent_simulation.py
```

---

## Cau truc thu muc
```
├── solution.py              # ETL Pipeline script
├── raw_data.json            # Input data
├── processed_data.csv       # Output sau ETL
├── generate_garbage.py      # Tao du lieu "rac"
├── garbage_data.csv         # Du lieu co loi chat luong
├── agent_simulation.py      # Stress test agent
├── experiment_report.md     # Bao cao thi nghiem
└── README.md                # File nay
```

---

## Ket qua
- Tong 5 records dau vao: 3 records hop le, 2 records bi loai (price <= 0 va category rong).
- Output `processed_data.csv` co them `discounted_price` va `processed_at`.
