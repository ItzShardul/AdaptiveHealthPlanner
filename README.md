# 🥗 Adaptive Health Planner

**Adaptive Health Planner** is a comprehensive, data-driven Android application designed to help users manage their physical health and daily nutrition.  

Unlike simple calorie counters, this app uses **professional formulas (Mifflin-St Jeor Equation)** and a **large local dataset of 1000+ food items** to provide a fully personalized health ecosystem.

---

# 🚀 Application Walkthrough

---

## 📍 Page 1: User Profile Setup (The Foundation)

The journey begins with a detailed health profile where the app collects the user's **"Physical Identity."**

### 🔹 Features:
- 🖼️ **Circular Profile Picture**  
  Uses implicit intent to fetch images from the device gallery.

- 🎨 **High-Contrast UI**  
  Important fields (Name, Age, Weight, Height) use white text on dark green containers for better readability.

- 🔄 **Smart Unit Converters**  
  Real-time conversion between:
  - Metric (Kg / cm)
  - Imperial (lbs / feet)

- 🧮 **BMI Engine**  
  Automatically calculates BMI and assigns category:
  - Underweight
  - Normal
  - Overweight
  - Obese

### 🔹 Buttons:
- **Select Picture** → Opens system gallery  
- **Save Profile** → Validates inputs and stores data using SharedPreferences  

---

## 📍 Page 2: Smart Food Selector (The Entry)

Users log their daily intake through a powerful search-based system.

### 🔹 Features:
- 🔍 **Search & Filter Engine**  
  Uses `AutoCompleteTextView` to search through **1000+ Indian food items**

- 🧪 **Nutrient Extraction**  
  Fetches:
  - Calories  
  - Protein  
  - Carbohydrates  
  - Fats  
  from a CSV-powered SQLite database  

### 🔹 Buttons:
- ⬅️ **Back Arrow** → Return to Profile  
- 📊 **View Macro Tracker** → Submit and open dashboard  
- ⚙️ **Update Info** → Modify profile  

---

## 📍 Page 3: Daily Macro Dashboard (The Brain)

The central hub where users track health progress in real-time.

### 🔹 Features:
- 📊 **BMI Status Hub** → Displays BMI value  
- 💡 **Motivational Tips** → Random health tip generator  
- 📈 **Visual Macro Tracker**  
  Progress bars for:
  - Calories  
  - Protein  
  - Carbs  
  - Fats  

- ⚠️ **Smart Nutrient Alerts**  
  Example:  
  `⚠️ Calorie limit exceeded!`

- 🔍 **Pinch-to-Zoom BMI Chart**  
  Interactive chart with color legend:
  - Blue → Underweight  
  - Green → Normal  
  - Yellow → Overweight  
  - Red → Obese  

### 🔹 Buttons:
- ⚙️ **Settings** → Modify profile  
- 📜 **Detailed History Log** → Open history page  

---

## 📍 Page 4: Detailed History Log (The Vault)

A professional tracking system for long-term analysis.

### 🔹 Features:
- 📅 **Calendar View**  
  Select any past date  

- 📋 **Tabular Log**  
  Displays:
  Meal Time | Food Name | Calories | Protein | Carbs | Fats
  
- 🔗 **Data Persistence**  
Uses SQL JOIN queries to link:
- User logs  
- Nutrition database  

### 🔹 Buttons:
- 🔍 **View History Log** → Fetch data  
- 🗑️ **Clear Log for Selected Day**  
Shows confirmation AlertDialog before deletion  

---

# 📊 The Daily Macro Tracker

## 🔹 What is it?

A visualization tool that tracks:
- Calories  
- Protein (P)  
- Carbohydrates (C)  
- Fats (F)  

It uses the **Mifflin-St Jeor Equation (BMR)** and adjusts values based on user goals:
- Lose Weight  
- Gain Muscle  
- Stay Fit  

---

## 🔹 Significance

1. 🎯 **Personalized Precision**  
 No generic limits — fully customized for each user  

2. 💪 **Goal Alignment**  
 Adjusts nutrients based on fitness goal  

3. ⚠️ **Prevents Overeating**  
 Smart alerts act as a virtual coach  

4. 📊 **Data Visualization**  
 Progress bars make data easy to understand  

---

# 🛠️ Mapping of Curriculum Practicals

| Practical | Feature Implementation | Location |
|----------|----------------------|----------|
| 1. SharedPreferences | Store profile & skip setup | ProfileActivity |
| 2. Logic / Generator | Mifflin-St Jeor calculation | MainActivity |
| 3. UI Layouts | ConstraintLayout, ScrollView, TableLayout | XML Files |
| 4. Event Handling | Validation, unit conversion, search | Multiple Activities |
| 5. Intents | Navigation + Image Picker | All Activities |
| 6. Dialog & Notifications | Delete confirmation + alerts | HistoryActivity |
| 7. SQLite Database | Food DB + logs + JOIN queries | DatabaseHelper |
| 8. Extra Features | Zoom chart, alerts, converters | Multiple Screens |

---

# 🛠️ Tech Stack

- 💻 **Language:** Java  
- 🗄️ **Database:** SQLite  
- 💾 **Storage:** SharedPreferences  
- 🎨 **UI:** Material Design 3  
- 📦 **Components:**  
- CircleImageView  
- TableLayout  
- CalendarView  

- 📱 **Minimum SDK:** 26 (Android 8.0)

---

# 🌟 Key Highlights

- ✔️ 1000+ food dataset  
- ✔️ Real-time macro tracking  
- ✔️ Smart alerts system  
- ✔️ Interactive UI & charts  
- ✔️ Fully offline functionality  

---

# 🚀 Future Improvements

- AI-based food recommendations  
- Barcode food scanning  
- Cloud sync (Firebase)  
- Wearable integration  

---

# 📌 Conclusion

Adaptive Health Planner is not just a tracker — it is a **complete personalized health ecosystem** that combines:
- Nutrition  
- Fitness  
- Data intelligence  

into a single smart Android application.

---
