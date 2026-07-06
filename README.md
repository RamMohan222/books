# Books
Programming Books
## Repository
- [Design Patterns](https://github.com/iluwatar/java-design-patterns/tree/master)
- [System Desing]()
- [JVM Options ChrisWhoCodes](https://chriswhocodes.com/)

#### 1. Memorize these numbers:

| Name       |            Number | Scientific notation |
| ---------- | ----------------: | ------------------: |
| 1 Thousand |             1,000 |              (10^3) |
| 1 Million  |         1,000,000 |              (10^6) |
| 1 Billion  |     1,000,000,000 |              (10^9) |
| 1 Trillion | 1,000,000,000,000 |           (10^{12}) |


```txt
# Memory:
1 KB ≈ 10^3 bytes
1 MB ≈ 10^6 bytes
1 GB ≈ 10^9 bytes
1 TB ≈ 10^12 bytes
1 PB ≈ 10^15 bytes

# Numbers: 
1 Thousand = 10^3
1 Million = 10^6
1 Billion = 10^9
1 Trillion = 10^12
```

#### 2. Storage Calculation:
```txt
# Storage Formula:
Storage = Number of records × Size of one record
```

*Example 1: To store 100 million records/ each record size is 100 bytes*
```txt
100 million × 100 bytes
= 100 × 10^6 × 10^2
= 10^10 bytes
= 10 GB
```
*Example 2: 100 million records/day / each records size is 100 bytes to store for 10 years*
```txt
# Total records
100 million × 365 × 10
= 10^2 * 10^6 * 365 * 10^1
= 10^9 * 365
= 365 billion records

# For storage
365 billion × 100 bytes
= 365 × 10^9 × 10^2
= 36.5 × 10^12 bytes
≈ 36.5 TB
```

#### 3. Data Rate Formula:
```txt
                    Operations/day
Operations/sec  =  ----------------
                     24 × 3600
```
*Example 1:*
```txt
                      100,000,000
100 million/day  =   ------------  ≈ 1157/sec  (round 1160/sec)
                       86,400
```

#### 4. Bandwidth Formula:
```txt
Bandwidth = Requests/sec × Request Size
```
*Example 1:*
```txt
10,000 requests/sec
Each Request Size = 2 KB

Bandwidth = 10,000 × 2 KB = 20 MB/sec
```

#### 5. RAM Formula:
```txt
RAM = Objects in memory × Size of one object
```
*Example 1:*
```txt
5 million cache entries
Each = 200 bytes

RAM = 5 × 10^6 × 200
    = 10^9 bytes
    ≈ 1 GB
```

#### 6. Quick Mental Math
```txt
# Instead of writing all the zeros:

Million = 10^6
Billion = 10^9

100 bytes = 10^2

1 KB = 10^3
1 MB = 10^6
1 GB = 10^9
1 TB = 10^12

# Example:
500 million records
200 bytes each

500 × 10^6 × 2 × 10^2

= 1000 × 10^8 (10^11 bytes)
= 100 * 10^1 * 10^8
= 100 * 10^9 bytes
= 100 GB
```

#### 7. Common System Design Sizes
| Item                   |  Approx. Size |
| ---------------------- | ------------: |
| Character              |        1 byte |
| UUID                   |      16 bytes |
| Timestamp              |       8 bytes |
| Integer                |       4 bytes |
| Long                   |       8 bytes |
| URL                    | 100–200 bytes |
| Email                  |   20–50 bytes |
| Username               |   20–40 bytes |
| Small JSON object      |      0.5–2 KB |
| Image thumbnail        |     20–100 KB |
| HD photo               |        2–5 MB |
| 1080p video (1 minute) |     50–100 MB |

--------

# Converting Requests per Day to Requests per Second

## Formula

```
                Requests/day
Requests/sec = -------------- 
                24 * 60 * 60

                Requests/day
Requests/sec = -------------- 
                   86,400
```

## Example: 1 Million Requests/Day
```txt
                1,000,000
Requests/sec = -------------- ≈ 11.57
                 86,400
```

**Answer:** ≈ **11.6 requests/second** (round to **12 requests/sec**)

---

## Quick Reference

| Requests/Day | Requests/Second (Approx.) |
|--------------|--------------------------:|
| 1 Million    | 12/sec                    |
| 10 Million   | 116/sec                   |
| 100 Million  | 1,160/sec                 |
| 1 Billion    | 11,600/sec                |

---

## Mental Shortcut

Since:
```
                1,000,000
Requests/sec = ----------- ≈ 11.57 (round to 12)
                 86,400
```

You can remember:

- **1 Million/day ≈ 12 requests/sec**
- **10 Million/day ≈ 120 requests/sec**
- **100 Million/day ≈ 1,200 requests/sec**
- **1 Billion/day ≈ 12,000 requests/sec**

These rounded values are commonly used for back-of-the-envelope estimations in system design interviews.
