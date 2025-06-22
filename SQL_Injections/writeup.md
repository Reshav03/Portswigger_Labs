![Image1](../SQL_Injections/images/Example1.jpg)

<H2><B>What is SQL injection (SQLi)?</B></H2>

This can allow an attacker to view data that they are not normally able to retrieve. This might include data that belongs to other users, or any other data that the application can access. In many cases, an attacker can modify or delete this data, causing persistent changes to the application's content or behavior.

<H2><B>How to detect SQL injection vulnerabilities?</B></H2>

🔍 1. Manual Detection Techniques
These methods work when you have access to the application's frontend (e.g., login forms, URL parameters, search bars).

✅ Input Fields to Test:
Login forms

Search bars

Contact forms

URL parameters (GET requests)

Cookies or HTTP headers (advanced)

🧪 Common Payloads to Try:

## 🧪 Common Payloads to Try

| Payload                        | Purpose                                |
|-------------------------------|----------------------------------------|
| `' OR '1'='1`                 | Bypass login or cause always true condition |
| `admin' --`                   | Comment out rest of query              |
| `admin' #`                    | Alternative comment style              |
| `' UNION SELECT NULL, NULL--` | Test for UNION-based injection         |
| `' OR 1=1 LIMIT 1 OFFSET 1--` | Pagination-based injection             |
| `1' AND SLEEP(5)--`           | Time-based blind SQLi                  |

---

### ✅ Start small:

```sql
sql
' --


