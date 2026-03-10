# NOMI – SIT Test Run Report

---

## 1️⃣ Test Run Information

- **Project Name:** NOMI – One Evidence Synthesis Platform
- **Test Cycle:** DEV Env V1.0
- **Build Version:** v1.0.0
- **Environment:** DEV
- **Execution Start Date:** 02-Mar-2026
- **Execution End Date:** 
- **Executed By:** Dinesh Subramaniyan

---

## 2️⃣ Test Execution Summary

| Total Test Cases | Executed | Passed | Failed | Blocked | Not Executed |
|------------------|----------|--------|--------|---------|--------------|
|      29          |      08  | 07     |    01  | 01      |           21 |

---

## 3️⃣ Detailed Test Case Execution Status

| TC ID | Test Case Name | Status | Defect ID | Comments |
|-------|----------------|--------|-----------|----------|
| TC_001 | Validating Valid Username and Password | ✅ Passed | — | Working as expected |
| TC_002 | Validating valid Username, Empty Password | ✅ Passed | - | Working as expected |
| TC_003 | alidating Valid Username and Invalid Password | ✅ Passed | — | As expected |
| TC_004 | Validating User accessing the NOMI Application from other environment | ✅ Passed | — | Working as expected  |
| TC_005 | Validating without user name if user clicks the nect button | ✅ Passed | - | Working as expected  |
| TC_006 | Validating the error message while entering the invalid domain name in mail address | ✅ Passed | — | Working as expected  |
| TC_007 | Validating the error message while entering the invalid username and correct Domain name | ✅ Passed | — | Working as expected |
| TC_008 | Validating the Home Page | ✅ Passed | — | Working as expected |
| TC_009 | Validating Valid PDF Upload Through File Browser |  ❌ Failed | GPDDDTME-337 | Facing issue after uplaoding the file |

---

## 4️⃣ Defect Summary

| Defect ID | Severity | Status | Description |
|-----------|----------|--------|------------|
|GPDDDTME-337| High |Dev inprocess|Structure Summary and Quality Score Not Populating|
|GPDDDTME-338| High | Dev In process |Recent Files Toggle Bar Misaligned in Upload and Preview Pages |
|GPDDDTME-314| High | Dev In process| Result payload is still unavailable while uploading "LOVE-CD D'Haens UEG Week 2024.pdf|


---

## 5️⃣ Observations

- SSO login working as expected.
- Facing issue after uploading 
- Recent Files Toggle Bar Misaligned in Upload and Preview Pages
- Result payload is still unavailable while uploading "LOVE-CD D'Haens UEG Week 2024.pdf


---

## 6️⃣ Risks / Blockers

- Audit and uploading getting error

---

## 7️⃣ Overall Test Run Status



---