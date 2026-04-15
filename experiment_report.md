# Experiment Report: Data Quality Impact on AI Agent

**Student ID:** AI20K-XXXX
**Name:** (Dien ten cua ban)
**Date:** 2026-04-15

---

## 1. Ket qua thi nghiem

Chay `agent_simulation.py` voi 2 bo du lieu va ghi lai ket qua:

| Scenario | Agent Response | Accuracy (1-10) | Notes |
|----------|----------------|-----------------|-------|
| Clean Data (`processed_data.csv`) | Agent: Based on my data, the best choice is Laptop at $1200. | 9 | Gia tri hop ly, dung theo du lieu sach. |
| Garbage Data (`garbage_data.csv`) | Agent: Based on my data, the best choice is Nuclear Reactor at $999999. | 2 | Bi outlier keo lech, khong thuc te. |

---

## 2. Phan tich & nhan xet

### Tai sao Agent tra loi sai khi dung Garbage Data?

Khi dung garbage data, agent dua tren quy tac don gian “chon gia cao nhat trong category electronics”. Bo du lieu rac co nhieu loi: duplicate IDs lam lech thong ke, wrong data type (gia chuoi “ten dollars”) co the bi bo qua hoac doc sai, outliers nhu “Nuclear Reactor” gia qua lon lam sai lech ket qua, va null values lam giam chat luong du lieu. Vi agent khong co co che kiem tra/lam sach, no tin tuong du lieu sai va tra loi thieu thuc te. Data quality kem dan den sai lech logic va giam do tin cay cua he thong.

---

## 3. Ket luan

**Quality Data > Quality Prompt?** Dong y. Du prompt co tot den dau, neu du lieu dau vao rac thi ket qua van sai. Du lieu sach giup agent suy luan dung va on dinh hon.
