# 🗳️ Tideman (Ranked-Choice Voting System)

## 📌 Project Overview
This project is a sophisticated implementation of the **Tideman voting method** (also known as "Ranked Pairs"). It is a complex election system designed to guarantee a **"Condorcet winner"** if one exists. Unlike simple plurality voting, Tideman effectively avoids "spoiler effects" by allowing voters to rank candidates in order of preference.

---

## 🧠 The Challenge
The primary technical hurdle of this project was solving the **cycle detection problem** in a directed graph. As the algorithm locks in pairs of candidates based on their strength of victory, it must rigorously ensure that no circular dependencies (cycles) are created, which would otherwise result in a stalemate.

---

## 🛠️ Key Features & Implementation

* **Preference Mapping:** Developed a robust system to record and aggregate voter preferences across all candidates using multi-dimensional arrays.
* **Strength of Victory Logic:** Implemented a sorting mechanism to rank candidate pairs by their margin of victory, ensuring the most decisive results are prioritized.
* **Cycle Detection (Recursion):** Designed and implemented a **recursive algorithm** to traverse directed graphs and detect potential cycles before "locking" any pair.
* **Source Determination:** Engineered logic to identify the "Source" of the graph (the candidate with no incoming edges) to definitively declare the election winner.

---

## 💻 Technical Stack

* **Language:** `C`
* **Concepts:** Recursion, Adjacency Matrices, Directed Graphs, Sorting Algorithms, Memory Management.

---

## 🚀 How to Run

1.  **Compile the program:**
    ```bash
    make tideman
    ```
2.  **Execute the program with candidates:**
    ```bash
    ./tideman Alice Bob Charlie
    ```
3.  **Input the number of voters and their ranked preferences as prompted.**

---

## 🎓 Context
This project was completed as part of **Harvard University's CS50x: Introduction to Computer Science**, representing one of the most mathematically and logically challenging problem sets in the curriculum.
