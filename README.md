# Nutrition Tracker Pro

A robust, lightweight Python desktop application built using `tkinter` to log, track, and analyze daily macronutrient intake. Engineered using the **MoSCoW prioritization framework** and a **Software Completeness Specification**, this application provides rapid standalone utility with zero external dependencies, robust data type validation, and an automated local storage persistence layer.

---

## 🚀 Features & Capabilities

### 🔴 Must-Have Core Engine

* **Dual Macro Aggregation:** Dedicated, real-time calculation fields tracking total grams for both **Protein** and **Carbohydrates**.
* **Food Item Descriptions:** Explicit labeling capability to associate naming tags with specific logged macro entries.
* **Caloric Thermodynamic Derivation:** Dynamic calculations running the precise biological equation to update total intake tracking instantly:

$$\text{Calories} = (\text{Protein} \times 4) + (\text{Carbohydrates} \times 4)$$



### 🟡 Should-Have Usability & Validation

* **Target Daily Quotas:** Fully adjustable baseline configuration inputs to set customized personal caps for daily protein and carbohydrate intake.
* **Visual Metric Dashboard:** Responsive visual progress meters that scale dynamically to display active consumption ratios.
* **Data Sanitation & Fault Inversion:** Multi-layered input filtering that handles empty data fields, out-of-bounds metrics ($>1500\text{g}$), and structural text injection errors without breaking the application.
* **Interactive Transaction Ledger:** Chronological data display grid detailing the custom meals logged during the active tracking session.

### 🟢 Could-Have State Persistence

* **JSON Local Database Engine:** Zero-config automatic state saving to a local `nutrition_data.json` flat-file file structure. Your targets and logs load seamlessly between software system reboots.
* **Granular Deletion Operations:** Interactive item extraction allowing users to highlight a row in the transaction grid and remove it, adjusting current macro metrics instantly.

---

## 🛠️ Tech Stack & Architecture

* **Language:** Python 3.x
* **GUI Engine:** `tkinter` / `ttk` (Clam native theme style engine)
* **Storage Backend:** Flat-File Local JSON
* **OS Portability:** Cross-platform support across Windows, macOS, and Linux out-of-the-box.

---

## 📦 Installation & Execution

Ensure you have a modern deployment environment running Python 3. Clone the source repository, navigate into the destination directory, and execute the file layout loop:

```bash
# Clone the repository
git clone https://github.com/wayneeffect/Nutrition-Tracker-Pro.git

# Navigate to the project folder
cd Nutrition-Tracker-Pro

# Spin up the application engine
python nutrition_tracker_pro.py

```

No external `pip` dependencies are required. The software relies strictly on built-in standard library utilities (`json`, `os`, and `tkinter`) to maximize operational security and deployment speeds.

---

## 🧬 Architectural Strategy Applied

This project represents a structural shift from traditional, multi-week release lifecycles into a hyper-compressed, high-velocity development loop. By utilizing precise prompt-engineering logic maps, the software moved from initial ideation to a fully complete MVP—complete with comprehensive error wrappers and a local data validation tier—in under 15 minutes.
