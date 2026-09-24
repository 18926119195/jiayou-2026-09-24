# cost_calc.py

> **路径**: `cost_calc.py`  
> **分类**: 代码  
> **大小**: 1.7 KB  
> **最后修改**: 2026-09-24T09:23:08.140Z  

## 文件开头预览

```py
tokens = [
    (160128, 215, 7233),   # Z1-Q1
    (160128, 211, 6897),    # Z1-Q2
    (160000, 338, 8298),    # Z1-Q3
    (160000, 338, 13947),   # Z1-Q4
    (160000, 345, 6692),    # Z2-Q1
    (160000, 343, 12310),   # Z2-Q2
    (160000, 350, 17283),   # Z2-Q3
    (160000, 343, 9525),    # Z2-Q4
    (160128, 222, 9981),    # Z3-Q1
    (160128, 214, 13694),   # Z3-Q2
    (160000, 342, 9655),    # Z3-Q3
    (160000, 341, 16684),   # Z4-Q1
    (160000, 345, 10616),   # Z4-Q2
    (160000, 349, 8819),    # Z4-Q3
    (160000, 342, 5508),    # Z4-Q4
]
qids = ['Z1-Q1','Z1-Q2','Z1-Q3','Z1-Q4','Z2-Q1','Z2-Q2','Z2-Q3','Z2-Q4','Z3-Q1','Z3-Q2','Z3-Q3','Z4-Q1','Z4-Q2','Z4-Q3','Z4-Q4']

print("=== PEAK pricing (h=0.006, m=0.30, o=1.20) ===")
h = 0.006; m = 0.30; o = 1.20
total = 0
for i in range(15):
    ch, cm, ct = tokens[i]
    cost = ch/1e6*h + cm/1e6*m + ct/1e6*o
    total += cost
    print(f"{qids[i]}: ${cost:.5f}  (CNY {cost*7.2:.3f})")
print(f"\nTotal USD: ${total:.5f}")
print(f"Total CNY @7.2: {total*7.2:.3f}")
print(f"Total CNY @7.3: {total*7.3:.3f}")

print("\n=== NON-PEAK pricing (h=0.003, m=0.15, o=0.60) ===")
h = 0.003; m = 0.15; o = 0.60
total2 = 0
for i in range(15):
    ch, cm, ct = tokens[i]
    cost = ch/1e6*h + cm/1e6*m + ct/1e6*o
    total2 += cost
    print(f"{qids[i]}: ${cost:.5f}  (CNY {cost*7.2:.3f})")
print(f"\nTotal USD: ${total2:.5f}")
print(f"Total CNY @7.2: {total2*7.2:.3f}")
print(f"Total CNY @7.3: {total2*7.3:.3f}")

print("\n=== Key breakdown ===")
ch_total = sum(t[0] for t in tokens)
cm_total = sum(t[1] for t in tokens)
ct_total = sum(t[2] for t in tokens)
print(f"Total cache hit:  {ch_total:,}")
print(f"Total cache miss: {cm_total:,}")
print(f"Total completion: {ct_total:,}")
```
