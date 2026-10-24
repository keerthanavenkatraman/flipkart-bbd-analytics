## Seed row-count verification

| Table | Expected rows |
| --- | ---: |
| reps | 4 |
| products | 9 |
| customers | 24 |
| orders | 90 |

## q01 — Query Results

- Expected row count: 19
- Actual row count: 19
- Status: PASS

| order\_id | customer\_id | item | amount |
| --- | --- | --- | --- |
| 1001 | 10 | Bluetooth Speaker |  |
| 1002 | 16 | Smart Watch | 4500 |
| 1004 | 19 | Cotton Kurta | 2800 |
| 1010 | 19 | Wireless Earbuds |  |
| 1033 | 18 | Denim Jacket | 2500 |
| 1035 | 5 | Bluetooth Speaker | 2800 |
| 1036 | 22 | Denim Jacket | 5000 |
| 1037 | 3 | Bedsheet Set | 3800 |
| 1042 | 14 | Table Lamp | 1100 |
| 1044 | 10 | Running Shoes | 3600 |
| 1052 | 15 | Smart Watch | 13500 |
| 1057 | 4 | Bluetooth Speaker | 2800 |
| 1058 | 13 | Bedsheet Set | 1900 |
| 1063 | 10 | Air Fryer | 5200 |
| 1064 | 20 | Bluetooth Speaker |  |
| 1068 | 23 | Air Fryer | 5200 |
| 1071 | 22 | Air Fryer | 5200 |
| 1075 | 4 | Running Shoes | 3600 |
| 1078 | 3 | Cotton Kurta | 1400 |

## q02 — Query Results

- Expected row count: 3
- Actual row count: 3
- Status: PASS

| order\_id | customer\_id | item | status |
| --- | --- | --- | --- |
| 1001 | 10 | Bluetooth Speaker | pending |
| 1010 | 19 | Wireless Earbuds | pending |
| 1064 | 20 | Bluetooth Speaker | pending |

## q03 — Query Results

- Expected row count: 5
- Actual row count: 5
- Status: PASS

| order\_id | customer\_id | item | amount |
| --- | --- | --- | --- |
| 1061 | 16 | Air Fryer | 15600 |
| 1065 | 22 | Air Fryer | 15600 |
| 1069 | 15 | Air Fryer | 15600 |
| 1077 | 3 | Air Fryer | 15600 |
| 1006 | 5 | Smart Watch | 13500 |

## q04 — Query Results

- Expected row count: 8
- Actual row count: 8
- Status: PASS

| customer\_id | first\_name | last\_name | region | age |
| --- | --- | --- | --- | --- |
| 24 | Reena | Kulkarni | West | 25 |
| 8 | Divya | Gupta | West | 26 |
| 17 | Farhan | Shah | North | 27 |
| 1 | aarav | Sharma | North | 28 |
| 16 | Nisha | Mishra | West | 36 |
| 5 | Vikram | Singh | North | 37 |
| 12 | Pooja | Menon | West | 39 |
| 21 | Manoj | Desai | North | 40 |

## q05 — Query Results

- Expected row count: 1
- Actual row count: 1
- Status: PASS

| total\_orders | total\_revenue | avg\_order\_value | min\_order\_value | max\_order\_value |
| --- | --- | --- | --- | --- |
| 63 | 346200 | 5495.2381 | 1100 | 15600 |

## q06 — Query Results

- Expected row count: 3
- Actual row count: 3
- Status: PASS

| status | number\_of\_orders | total\_amount |
| --- | --- | --- |
| completed | 63 | 346200 |
| pending | 19 | 64900 |
| disputed | 8 | 73200 |

## q07 — Query Results

- Expected row count: 4
- Actual row count: 4
- Status: PASS

| item | number\_of\_orders | revenue |
| --- | --- | --- |
| Air Fryer | 9 | 104000 |
| Smart Watch | 9 | 67500 |
| Wireless Earbuds | 11 | 60800 |
| Running Shoes | 8 | 43200 |

## q08 — Query Results

- Expected row count: 4
- Actual row count: 4
- Status: PASS

| region | number\_of\_customers | average\_age | min\_age | max\_age |
| --- | --- | --- | --- | --- |
| East | 6 | 34.0000 | 29 | 41 |
| North | 6 | 37.5000 | 27 | 48 |
| South | 6 | 36.3333 | 24 | 52 |
| West | 6 | 28.5000 | 22 | 39 |

## q09 — Query Results

- Expected row count: 90
- Actual row count: 90
- Status: PASS

| order\_id | order\_month | first\_name | last\_name | region | rep\_name | item | quantity | amount | status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1001 | 2026-09 | MEERA | Patil | South | Kavya Nair | Bluetooth Speaker | 2 |  | pending |
| 1002 | 2026-09 | Nisha | Mishra | West | Neha Kulkarni | Smart Watch | 1 | 4500 | pending |
| 1003 | 2026-09 | Lakshmi | Kapoor | South | Kavya Nair | Air Fryer | 2 | 10400 | disputed |
| 1004 | 2026-09 | Gaurav | Yadav | East | Sanjay Roy | Cotton Kurta | 2 | 2800 | pending |
| 1005 | 2026-09 | Tanvi | Thakur | South | Kavya Nair | Table Lamp | 1 | 1100 | completed |

* Showing the first 5 of 90 rows here. Export all 90 rows to `data/orders_enriched.csv` as a separate deliverable.

## q10 — Query Results

- Expected row count: 4
- Actual row count: 4
- Status: PASS

| customer\_id | first\_name | last\_name | region |
| --- | --- | --- | --- |
| 6 | Ananya | Reddy | South |
| 11 | Imran | Joshi | East |
| 17 | Farhan | Shah | North |
| 24 | Reena | Kulkarni | West |

## q11 — Query Results

- Expected row count: 12
- Actual row count: 12
- Status: PASS

| region | order\_month | number\_of\_orders | number\_of\_customers | total\_revenue | average\_revenue |
| --- | --- | --- | --- | --- | --- |
| East | 2026-09 | 2 | 2 | 6400 | 3200.0000 |
| East | 2026-10 | 4 | 3 | 12200 | 3050.0000 |
| East | 2026-11 | 6 | 5 | 50900 | 8483.3333 |
| North | 2026-09 | 8 | 2 | 53500 | 6687.5000 |
| North | 2026-10 | 6 | 4 | 41300 | 6883.3333 |
| North | 2026-11 | 5 | 4 | 24500 | 4900.0000 |
| South | 2026-09 | 5 | 3 | 19800 | 3960.0000 |
| South | 2026-10 | 5 | 4 | 19000 | 3800.0000 |
| South | 2026-11 | 7 | 4 | 43700 | 6242.8571 |
| West | 2026-09 | 4 | 3 | 18600 | 4650.0000 |
| West | 2026-10 | 5 | 4 | 20600 | 4120.0000 |
| West | 2026-11 | 6 | 3 | 35700 | 5950.0000 |

## q12 — Query Results

- Expected row count: 9
- Actual row count: 9
- Status: PASS

| item | total\_revenue | contribution\_tier |
| --- | --- | --- |
| Air Fryer | 104000 | High |
| Smart Watch | 67500 | High |
| Wireless Earbuds | 60800 | High |
| Running Shoes | 43200 | Medium |
| Denim Jacket | 17500 | Medium |
| Cotton Kurta | 16800 | Medium |
| Bluetooth Speaker | 14000 | Low |
| Bedsheet Set | 11400 | Low |
| Table Lamp | 11000 | Low |

## q13 — Query Results

- Expected row count: 12
- Actual row count: 12
- Status: PASS

| rep\_name | order\_month | monthly\_target | revenue | performance\_tier |
| --- | --- | --- | --- | --- |
| Arjun Mehta | 2026-09 | 40000 | 53500 | Above Target |
| Arjun Mehta | 2026-10 | 40000 | 41300 | On Target |
| Arjun Mehta | 2026-11 | 40000 | 24500 | Below Target |
| Kavya Nair | 2026-09 | 20000 | 19800 | Below Target |
| Kavya Nair | 2026-10 | 20000 | 19000 | Below Target |
| Kavya Nair | 2026-11 | 20000 | 43700 | Above Target |
| Neha Kulkarni | 2026-09 | 20000 | 18600 | Below Target |
| Neha Kulkarni | 2026-10 | 20000 | 20600 | On Target |
| Neha Kulkarni | 2026-11 | 20000 | 35700 | Above Target |
| Sanjay Roy | 2026-09 | 12000 | 6400 | Below Target |
| Sanjay Roy | 2026-10 | 12000 | 12200 | On Target |
| Sanjay Roy | 2026-11 | 12000 | 50900 | Above Target |
