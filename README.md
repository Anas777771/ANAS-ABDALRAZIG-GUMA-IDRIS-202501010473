# Week 2 - Tutorial 2: Movie Theater Admission Policy

## 1. Identify the Components

### 1.1 Inputs

| Input | Type | Description |
|---------|---------|---------|
| age | Integer | User's age in years |
| is_with_adult | Boolean | True if accompanied by an adult |
| has_ticket | Boolean | True if user has a valid ticket |

### 1.2 Process

Check:

(age >= 13 OR is_with_adult) AND has_ticket

### 1.3 Output

- Allowed to enter
- Denied entry

---

## 2. Design the Algorithm

### 2.1 Flowchart

Start

↓

Read age, is_with_adult, has_ticket

↓

Check (age >= 13 OR is_with_adult)

↓

Check has_ticket

↓

Allowed to enter / Denied entry

↓

End

---

### 2.2 Truth Table

| A | B | C | Output |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 0 |
| 1 | 1 | 1 | 1 |

Where:
- A = age >= 13
- B = is_with_adult
- C = has_ticket

---

### 2.3 Algorithm

Step 1: Start

Step 2: Input age, is_with_adult, has_ticket

Step 3: Check

(age >= 13 OR is_with_adult) AND has_ticket

Step 4:
If True → Allowed to enter

Else → Denied entry

Step 5: End

---

### 2.4 Pseudocode

```text
BEGIN

INPUT age
INPUT is_with_adult
INPUT has_ticket

IF ((age >= 13 OR is_with_adult) AND has_ticket) THEN
    DISPLAY "Allowed to enter"
ELSE
    DISPLAY "Denied entry"
END IF

END
```

## 3. Evaluate Expression

### Test Case 1

Input:
- age = 15
- is_with_adult = False
- has_ticket = True

Output:
Allowed to enter

### Test Case 2

Input:
- age = 10
- is_with_adult = True
- has_ticket = True

Output:
Allowed to enter

### Test Case 3

Input:
- age = 10
- is_with_adult = False
- has_ticket = True

Output:
Denied entry

### Test Case 4

Input:
- age = 16
- is_with_adult = False
- has_ticket = False

Output:
Denied entry