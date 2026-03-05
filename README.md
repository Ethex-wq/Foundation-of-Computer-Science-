## Task 1 - Encoding Formats & Secure Data Exchange
This task explores encoding formats like Base64, Hex, and URL encoding and how 
they work with HTTPS, TLS, and SMTP for secure data transmission.

- **Base64** converts binary data to ASCII text, used in email attachments and JWTs, increases size by 33%
- **Hex** converts each byte to 2 characters, used in hash outputs and debugging, doubles data size
- **URL Encoding** replaces unsafe characters with % codes, for example space becomes %20
- **TLS Flow** - data is Base64 encoded, then encrypted with AES, sent over HTTPS, then decrypted and decoded at the server

---

## Task 2 - P vs NP & Seating Arrangement Problem
This task explains P vs NP using a classroom seating scenario where friends and 
same-city students cannot sit next to each other.

- **P problems** can be solved fast. Checking a seating plan is P - just scan each pair
- **NP problems** are hard to solve but easy to check. Finding a valid plan is NP
- **Brute Force** tries all arrangements (n!) - works for 5 students, impossible for 20+
- **Heuristic** places most-constrained students first - much faster but not always perfect

---

## Task 3 - Database Normalisation & SQL
This task fixes a flat club membership table using normalisation and SQL.

- **Problems found** - redundant data, update anomaly, insert anomaly, delete anomaly
- **1NF** - atomic values, composite key (StudentID + ClubName)
- **2NF** - split into Student, Club, and Membership tables
- **3NF** - no transitive dependencies, each column depends only on its primary key
- **SQL** - includes CREATE TABLE, INSERT, SELECT, and JOIN queries
- **ER Diagram** - Student and Club linked through Membership as many-to-many
