

# **Sorting Simulator — Operating Systems Project**

### *Parallel & Serial Sorting Visualization using SFML, OpenMP, and POSIX Threads*

---

## 📌 **Overview**

This project is an interactive **Sorting Simulator** built using **C++**, **SFML**, **OpenMP**, and **POSIX Threads**.
It visualizes the performance of multiple **serial**, **multithreaded**, and **OpenMP-based parallel sorting algorithms** on a dataset of **10,000 randomly generated student marks**.

The project includes a full graphical interface with menus, buttons, paging, and real-time execution time display.

---

## 🎯 **Objectives**

* Demonstrate how different sorting algorithms perform under:

  * Serial execution
  * Multithreading (POSIX Threads)
  * Parallel execution with **OpenMP**
* Visualize sorted/unsorted datasets using SFML
* Measure and display execution time for each method
* Display grade distribution based on sorted marks

---

## 🧩 **Features**

### ✔️ **Sorting Algorithms Implemented**

| Algorithm       | Serial | POSIX Threads | OpenMP |
| --------------- | ------ | ------------- | ------ |
| **Bubble Sort** | ✓      | ✓             | ✓      |
| **Merge Sort**  | ✓      | ✓             | ✓      |
| **Quick Sort**  | ✓      | ✓             | ✓      |

---

### ✔️ **Graphical Interface (SFML)**

* Main menu + submenus
* Button hover and click effects
* Background image support
* Paginated display (20 items per page)
* Execution time display window
* Grade distribution window

---

### ✔️ **Dataset**

* 10,000 student marks generated randomly from **1–1000**
* Stored in global array `data[10000]`

---

## 🛠️ **Technologies Used**

* **C++**
* **SFML 2.5+** (Graphics/UI)
* **OpenMP** (Parallel processing)
* **POSIX Threads (pthreads)** (Manual multithreading)
* **OOP concepts** (Buttons, pagination, UI)
* **Clock-based performance measurement**

---

## 📂 **Project Structure**

```
/your_project_folder
│── sorting_simulator.cpp   # Main source code
│── 1363709.png             # Background image
│── g-ari-bd.ttf            # Font file
│── README.md               # Documentation
```

---

## ⚙️ **How to Compile**

### **Linux (GCC/G++)**

Make sure SFML and pthreads are installed.

```bash
sudo apt install libsfml-dev
```

Compile using:

```bash
g++ sorting_simulator.cpp -o SortingSimulator \
    -lsfml-graphics -lsfml-window -lsfml-system \
    -fopenmp -lpthread
```

### **Windows (CodeBlocks / Visual Studio / MinGW)**

1. Install **SFML (2.5 or later)**
2. Link the following libraries:

   * `sfml-graphics`
   * `sfml-system`
   * `sfml-window`
   * `pthread`
3. Enable OpenMP (`-fopenmp` or `/openmp`)

---

## ▶️ **How to Run**

```bash
./SortingSimulator
```

---

## 🕹️ **Controls**

### **Main Menu**

* **Start** → Go to data fetch menu
* **Exit** → Quit program

### **Fetch Menu**

* Click **Fetch Data** to generate 10,000 marks
* After fetching, a window displays unsorted data

### **Sub Menu**

* **Quick Sort**
* **Merge Sort**
* **Bubble Sort**
* **Display Grades**

### **Inside Sorting Submenus**

You can choose:

* Serial version
* Parallel (threads) version
* OpenMP version

Each opens a new window showing:

* Sorted data
* Execution time
* Page navigation

  * ➡️ Right Arrow → Next Page
  * ⬅️ Left Arrow → Previous Page

### **Grades Window**

Shows count of:

* A (900+)
* B (800–899)
* C (700–799)
* D (600–699)
* F (<600)

---

## 📊 **Performance Output**

Each sorting window displays:

```
Total execution time: X.XXXX seconds
```

---

## ❗ Known Limitations

* SFML windows must stay open until the user closes them manually
* Single-core systems may not show large performance gains
* OpenMP QuickSort partitioning is not fully efficient (due to dependency issues)

---

## 👨‍💻 **Developed By**

* **Muhammad Huzaifa**
* **Usman Tanveer**
* **Hamza Haroon**



Just tell me!
