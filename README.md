# Optimized-parking-spot-allocation-using-a-novel-hybrid-algorithm

A smart parking management system that uses a grid-based layout and intelligent pathfinding algorithms to dynamically allocate parking spots and optimize exit decisions. Developed in Java using Swing for UI, the system supports real-time user interaction and compares multiple algorithms for performance.

---

## 🧠 Overview

Urban areas are facing severe parking challenges due to rising vehicle density, inefficient space usage, and lack of adaptive parking mechanisms. This project proposes an intelligent parking management solution using a combination of graph-based algorithms to enhance allocation speed, fairness, and exit efficiency in public lots like malls, offices, or metro stations.

The system:
- Categorizes parking slots into **short-term** and **long-term** zones.
- Uses **Dijkstra**, **Bellman-Ford**, **CBS**, **JPS**, and a novel **Combined Search Algorithm** to assign spots based on proximity, user needs, and lot availability.
- Compares the performance of algorithms in terms of **allocation time** and **path optimality**.
- Provides a **Java Swing-based UI** for vehicle selection, extension, and exit handling.
- Tracks overstays with a **timer system**, prompting reallocation or fine notices.

---

## 🧩 Project Structure

```
daa_project/
├── src/
│   └── main/java/com/mycompany/dsa/
│       ├── AllocationDisplay.java      # Dialogs and visual output
│       ├── AllocationPanel.java        # Main UI panel
│       ├── DSA.java                    # Entry point
│       ├── Edge.java                   # Edge representation for graph
│       ├── Graph.java                  # Grid graph logic
│       ├── Node.java                   # Grid node abstraction
│       ├── VehicleSelection.java       # UI for selecting vehicle type
│       └── module-info.java
├── target/                             # Compiled .class files
├── pom.xml                             # Maven project config
└── README.md
```

---

## 💻 Technologies Used

- **Java 17**
- **Java Swing** – for desktop GUI
- **Maven** – build & dependency management
- **Java AWT & Util** – for GUI and timer logic

---

## ⚙️ Algorithms Implemented

| Algorithm         | Purpose                                 | Highlights                                                  |
|------------------|-----------------------------------------|-------------------------------------------------------------|
| Dijkstra          | Shortest path to available slot         | Fast and efficient for uniform weights                      |
| Bellman-Ford      | Handles dynamic weights & edge cases    | More flexible than Dijkstra                                 |
| CBS (Content-Based Search) | Preference-aware allocation         | Considers user and space preferences                        |
| JPS (Jump Point Search) | Speed-optimized grid search           | Skips redundant nodes, faster traversal                     |
| Combined Search   | Hybrid of CBS + JPS                     | Achieves 15–25% better allocation time vs others            |

---

## 🖥️ UI Features

- 🚙 Vehicle Type Selection (Short-term or Long-term)
- 🕒 Timer-based Stay Tracking with Warnings
- 🔁 Extension Requests & Overstay Handling
- 🚪 Smart Exit Suggestion and Exit Validation
- ❌ Error Handling (e.g., wrong spot, full lot)
- 📊 Visual Feedback for Allocations via Dialogs

---

## 📊 Sample Outputs

- 📌 Dialogs for Parking Allocation from Entrances
- ⏰ Alerts for Timer Expiry or User Extension
- ❓ Wrong Spot / Full Lot messages
- 📈 Allocation Time Charts for Algorithm Comparison

> The **Combined Search Algorithm** consistently outperforms others in dynamic scenarios by intelligently blending user context and search optimization.

---

## 🧪 How to Run

### 1. Clone the repo
```bash
git clone https://github.com/your-username/parking-allocator.git
cd parking-allocator
```

### 2. Compile using Maven
```bash
mvn clean install
```

### 3. Run the Java Application
```bash
mvn exec:java -Dexec.mainClass="com.mycompany.dsa.DSA"
```

> You can also import the project into **IntelliJ**, **Eclipse**, or **NetBeans** as a Maven project and run directly.

---

## 📈 Results Summary

- Up to **25% improvement in allocation time** with Combined Search
- Enhanced UI experience using timer-based feedback
- All algorithms benchmarked on the same grid with consistent constraints

---

## 🚀 Future Scope

- 🛰️ Integrate IoT sensors for real-time slot detection
- 📱 Mobile/Web interface for remote bookings
- 💸 Dynamic pricing models based on demand
- 🤖 ML-based parking demand predictions
- 🚗 Autonomous vehicle integration

---

## 📄 License

This project is intended for academic and research use only.

