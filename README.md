Tideman (Ranked-Choice Voting System)
Project Overview
This project is an implementation of the Tideman voting method (also known as "Ranked Pairs"), which is a complex election system that guarantees a "Condorcet winner" if one exists. Unlike simple plurality voting, Tideman avoids "spoiler effects" by allowing voters to rank candidates in order of preference.

The Challenge
The core of this project is solving the problem of cycle detection in a directed graph. When locking in pairs of candidates based on their strength of victory, the algorithm must ensure that no circular dependencies (cycles) are created, which would make it impossible to determine a clear winner.

Key Features & Implementation
Preference Mapping: Developed a system to record and count voter preferences across all candidates in a multi-dimensional array.

Strength of Victory: Implemented logic to sort candidate pairs by the margin of victory, ensuring the most decisive wins are processed first.

Cycle Detection (Recursion): Designed a recursive algorithm to traverse a directed graph and prevent the creation of cycles before "locking" a victory.

Source Determination: Wrote logic to identify the "Source" of the graph (the candidate with no incoming edges) to declare the final winner.

Technical Stack
Language: C

Concepts: Recursion, Adjacency Matrices, Directed Graphs, Sorting Algorithms, Memory Management.
