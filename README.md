# 🩺 Smart Patient Symptom Tracker  
**Turning daily symptoms into real-time medical insights**

---

## 🚀 Overview

**Smart Patient Symptom Tracker** is a healthcare analytics prototype that transforms
daily patient-reported vitals and symptoms into **clear, time-based insights for doctors**.

Instead of relying on unreliable verbal recall during consultations, this system captures
structured health data over time and visualizes meaningful trends using **MongoDB time-series analytics**.

---

## 💡 Inspiration

In real-world clinical settings, doctors often ask questions like:

- “How long have you been feeling this pain?”
- “Was the fever getting better or worse?”
- “When did symptoms start?”

Patients usually answer from memory, which is often incomplete or inaccurate.

This project was inspired by the idea that:
> **Medical decisions should be based on trends, not memory.**

---

## 🧠 What the Project Does

### 👤 Patient View
- Patients enter daily health information such as:
  - Temperature
  - Pulse
  - Oxygen level (SpO₂)
  - Blood pressure
  - Blood sugar
  - Symptoms (fever, cough, fatigue, nausea, etc.)
  - Additional notes
- Calm **dark-themed UI** for comfortable daily use

### 🧑‍⚕️ Doctor Dashboard
- Doctors see:
  - A real-time snapshot of patient vitals
  - Automatically updating patient information
  - Historical trends visualized as charts
- Focuses on **clarity, not raw data overload**

---

## 🛠️ How It’s Built

### Frontend
- **HTML, CSS, Vanilla JavaScript**
- No frameworks, no backend server
- Runs locally by opening the HTML files

### Data & Analytics
- Health data is modeled as **time-series data**
- Each patient update is treated as a timestamped record
- Aggregations compute daily averages and trends
- Visualization is handled directly at the database level

### Visualization
- Charts are embedded directly into the dashboard
- No manual data processing or duplication
- Always reflects the latest stored data

---

## 🗄️ MongoDB Implementation (Core Technical Strength)

- Uses **time-series data modeling** for health metrics
- Designed for:
  - Append-only writes
  - Long-term patient monitoring
  - Efficient trend analysis
- Enables fast aggregation such as:

\[
\text{Daily Average} = \frac{1}{n} \sum_{i=1}^{n} x_i
\]

This allows doctors to reason over **patterns**, not isolated values.

---

## ⚡ Real-Time Prototype Behavior

- Patient updates propagate instantly to the doctor dashboard
- Simulates live monitoring without heavy infrastructure
- Production-ready architecture:
  - Frontend → API → MongoDB → Analytics → Dashboard

---

## 🚧 Challenges Faced

- Designing healthcare data as proper time-series records
- Keeping the UI medically informative but uncluttered
- Demonstrating real-time behavior without backend services
- Ensuring the demo remained realistic and scalable

---

## 📚 What I Learned

- Healthcare data naturally fits time-series models
- Flexible schemas are essential for evolving medical data
- Doctors value trends more than raw numbers
- Strong data modeling can be demonstrated even with a lightweight prototype

---

## 🔮 Future Scope

- Secure API-based data ingestion
- Multi-patient dashboards
- Alerts for abnormal trends
- Mobile application integration
- Compliance-ready deployment

---

## 🏁 Conclusion

**Smart Patient Symptom Tracker** demonstrates how modern data modeling and analytics
can significantly improve patient–doctor communication.

By converting daily symptom logs into meaningful trends, the project shows a clear path
from **data collection** to **clinical insight**.

> **Track symptoms. See trends. Treat better.**
