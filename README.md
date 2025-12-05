# Serutamba-Heritier-27141-SMRS-
Database Development PL/SQL Final Exam

# 🏥 Smart Medication Reminder System  
### Oracle PL/SQL Healthcare Automation Project  
**Student Name:** Serutamba Heritier  
**Student ID:** 27141  

---

## 📌 Overview
The **Smart Medication Reminder System** is an Oracle PL/SQL–based healthcare system designed to automate medication reminders, track missed doses, and generate adherence reports for hospitals and clinics.

This project follows the **8-phase capstone structure** required in INSY 8311.

---

# 🧩 PHASE I — Problem Identification
### **Problem**
Patients often forget to take medications on time, leading to treatment failure.

### **Solution**
A PL/SQL system that automates reminders and tracks dosage adherence.

### **Target Users**
- Doctors  
- Patients  
- Clinic administrators  
 

---

# 🧭 PHASE II — Business Process Modeling
Smart Medication Reminder System – Business Process Summary

The system automates medication scheduling and reminders in a healthcare environment, involving four actors: Patient, Doctor, System, and Database.

Workflow Summary

Patient Visit
The patient consults a doctor, initiating the care process.

Doctor Prescription
The doctor enters medication details (dosage, frequency, schedule) into the system.

System Processing
The system validates and stores the prescription in the database.

Automatic Trigger
When a prescription is stored, a trigger creates reminder schedules based on medication times.

Scheduled Monitoring
A timed PL/SQL procedure runs periodically to check which reminders are due.

Decision Check
The system compares the current time with reminder schedules to determine whether a reminder should be sent.

Reminder Delivery
If due, the system sends an alert to the patient via console, SMS, email, or other available channels.

MIS Relevance

Automates medication scheduling and reminders

Centralizes patient and prescription data

Supports decision-making through adherence tracking

Reduces manual workload for healthcare staff

Organizational Impact

Improves patient adherence and outcomes

Boosts efficiency by reducing manual tasks

Enables auditing and compliance monitoring

Provides data insights for health management

Analytics Opportunities

Medication adherence rates

Missed dose patterns

Reminder response trends

Doctor prescribing behaviors

Resource optimization based on patient activity



<img width="561" height="486" alt="BPMN" src="https://github.com/user-attachments/assets/a983208a-95ea-49bd-b574-c418e76d6a3e" />




---

# 🗂️ PHASE III — Logical Database Design
 ER Diagram
Entities:
- Patients  
- Doctors  
- Medicines  
- Prescriptions  
- Reminders  
- MissedDoses  

### Sample Data Dictionary Entry
| Table | Column | Type | Description |
|-------|--------|------|-------------|
| Patients | PatientID | NUMBER | Primary Key |
| Prescriptions | ReminderTime | DATE | Scheduled time |

<img width="564" height="529" alt="ERD" src="https://github.com/user-attachments/assets/1e3ca7fd-7c48-4428-b33d-757f92a8e24f" />

<img width="464" height="147" alt="8" src="https://github.com/user-attachments/assets/4b480bee-5306-4d06-beca-5832866fc782" />
<img width="234" height="139" alt="Capture" src="https://github.com/user-attachments/assets/f9eadc1e-867b-40ca-add4-3fd2c4d77cc5" />




---

# 🏛️ PHASE IV — Database Creation
### Tasks
- Create pluggable DB  
- Configure tablespaces  
- Create admin user  
- Set memory settings  
<img width="955" height="370" alt="Plugable" src="https://github.com/user-attachments/assets/aae2ecd3-ff66-4ab3-a434-97fb5f6a5c00" />
<img width="944" height="256" alt="tablespace" src="https://github.com/user-attachments/assets/58dff355-b0e5-4c44-a912-d74ebd5ebd27" />
<img width="945" height="181" alt="space" src="https://github.com/user-attachments/assets/addd0fa1-6be8-43e6-bd96-66428d0d542c" />
<img width="962" height="212" alt="admin" src="https://github.com/user-attachments/assets/c1ddc58d-a711-4c6d-81e1-5ded1aeb2f5e" />
<img width="963" height="263" alt="show" src="https://github.com/user-attachments/assets/2d60d11a-3059-4fdf-934f-33eb7f4ceec7" />
<img width="966" height="113" alt="memory" src="https://github.com/user-attachments/assets/4c450c55-69cf-4afe-bdd8-aa1797e0220f">


# 🧱 PHASE V — Table Implementation & Test Data

### ✔ Table Creation (DDL)
<img width="366" height="147" alt="1" src="https://github.com/user-attachments/assets/2b4cb47b-dd3d-4588-809a-299bbb4c860e" />
<img width="390" height="124" alt="2" src="https://github.com/user-attachments/assets/97c5d79b-4742-419a-8fa4-1ecc92720d81" />
<img width="273" height="143" alt="3" src="https://github.com/user-attachments/assets/83f65540-0263-41a6-9832-7a894162a2c2" />
<img width="577" height="172" alt="4" src="https://github.com/user-attachments/assets/04484a3d-ba53-4f56-901c-cc8ee3276ae4" />
<img width="242" height="174" alt="5" src="https://github.com/user-attachments/assets/b97be7db-2c7f-4eee-afd8-49cd7a7471e6" />
<img width="479" height="142" alt="6" src="https://github.com/user-attachments/assets/2dbeef9f-6580-4a33-ab02-95820544853c" />
<img width="639" height="154" alt="7" src="https://github.com/user-attachments/assets/b82fa9c4-0892-4dfe-807b-8c576091407b" />
<img width="464" height="147" alt="8" src="https://github.com/user-attachments/assets/e9ca20a2-2760-4195-a478-000518070219" />
<img width="700" height="172" alt="9" src="https://github.com/user-attachments/assets/da008c3f-4196-483b-bb04-f830533413d6" />
<img width="581" height="127" alt="DOCTOR" src="https://github.com/user-attachments/assets/8ab74411-76ba-4b7d-a0b7-a4d4d84bbaae" />
<img width="578" height="75" alt="DOCTORS" src="https://github.com/user-attachments/assets/d83cf488-4f77-41eb-99fb-ec07c299596b" />
<img width="573" height="106" alt="MEDICINE" src="https://github.com/user-attachments/assets/8a87162f-9d31-49fa-9eb8-cb1ce3de33b3" />
<img width="554" height="122" alt="MISSED_DOSES" src="https://github.com/user-attachments/assets/d58bfa78-ddec-4ace-9b3f-621544e1f55a" />
<img width="567" height="148" alt="PATIENT" src="https://github.com/user-attachments/assets/d8c1f778-5729-4a18-8dac-938ce903b060" />
<img width="573" height="82" alt="PATIENTS" src="https://github.com/user-attachments/assets/b558ffd1-e82a-4faa-98be-f5b4c1458202" />














```sql
CREATE TABLE Patients (
  PatientID NUMBER PRIMARY KEY,
  FullName VARCHAR2(100),
  Contact VARCHAR2(20),
  Age NUMBER,
  Gender VARCHAR2(10)
);

CREATE TABLE Doctors (
  DoctorID NUMBER PRIMARY KEY,
  FullName VARCHAR2(100),
  Specialization VARCHAR2(100)
);

CREATE TABLE Medicines (
  MedicineID NUMBER PRIMARY KEY,
  MedicineName VARCHAR2(100),
  Description VARCHAR2(200)
);

CREATE TABLE Prescriptions (
  PrescriptionID NUMBER PRIMARY KEY,
  PatientID NUMBER REFERENCES Patients(PatientID),
  DoctorID NUMBER REFERENCES Doctors(DoctorID),
  MedicineID NUMBER REFERENCES Medicines(MedicineID),
  Dosage VARCHAR2(50),
  TimesPerDay NUMBER,
  ReminderTime DATE
);

Phase VI: PL/SQL Development 🛠️

This phase focuses on creating PL/SQL objects (functions, procedures, and packages) to implement application logic on top of the existing database tables (Patients, Doctors, Medicines, Prescriptions).

Object Name	Type	Purpose
PK_MEDICATION_MANAGER	Package	Groups related PL/SQL functionality (such as FN_GET_DOCTOR_NAME, SP_LOG_MISSED_DOSE, SP_DOCTOR_SUMMARY_REPORT) for efficient compilation and code organization.
FN_GET_DOCTOR_NAME	Function	Returns the full name of a doctor based on DoctorID. Helps in reporting and display purposes.
SP_LOG_MISSED_DOSE	Procedure	Handles inserting records into a table for patients who missed a dose. Ensures proper transaction handling.
SP_DOCTOR_SUMMARY_REPORT	Procedure (Reporting)	Generates a summary report of prescriptions handled by a specific doctor. Uses explicit cursors and joins across multiple tables.
Key Notes

This phase does not modify the table structure; it adds PL/SQL logic on top of the existing schema.

All objects are encapsulated in the package PK_MEDICATION_MANAGER for modular and maintainable code.

Reporting and logging are separated from the core database tables for better clarity and debugging.
