# ECE 2112: Advanced Computer Programming and Algorithms
## Experiment 1: Introduction to Python Programming

**Student Name:** Bendicio, Sedric Lance B.
**Section:** 2ECE-A
**Date Submitted:** September 1, 2026  

---

## I. Objectives
The objectives of this laboratory activity are to:
1. Use basic Python functions, operators, and string operations.
2. Manipulate strings using indexing, slicing, and built-in string methods.
3. Apply extended sequence unpacking to manipulate the elements of a list.
4. Construct simple Python functions that return specified results without using external libraries, loops, or custom classes.

---

## II. Repository Contents
* `ECE2112_PA1.ipynb`: Jupyter Notebook containing the executed Python code, function implementations, and test case outputs.
* `README.md`: Overview, objective, and detailed discussion of the programming problems.

---

## III. Detailed Discussion of the Experiment

### Problem A: Word Rotation Problem (`rotate_word`)
* **Objective:** Take a non-empty string and move its first character to the end while keeping the rest of the characters in order and preserving original capitalization.
* **Implementation Strategy:** Utilized Python string slicing (`text[1:]`) to capture all characters from index 1 to the end, and string indexing (`text[0]`) to isolate the first character. Merged them using string concatenation (`text[1:] + text[0]`).
* **Example Output:** `rotate_word("python")` $\rightarrow$ `"ythonp"`

---

### Problem B: Username Builder Problem (`make_username`)
* **Objective:** Combine a first name and last name into a single standardized username format (`firstname.lastname`) in lowercase with all internal spaces removed.
* **Implementation Strategy:** 
  1. Applied the `.lower()` method to both input strings to ensure lowercase consistency.
  2. Applied `.replace(" ", "")` to strip any existing whitespace within multi-word names.
  3. Formatted the final output using string concatenation or f-strings joined by a period (`.`).
* **Example Output:** `make_username("Ana Maria", "De Leon")` $\rightarrow$ `"anamaria.deleon"`

---

### Problem C: Bookend Swap Problem (`swap_bookends`)
* **Objective:** Swap the first and last elements of a list containing at least two items while keeping the order of all middle elements intact, without modifying the original input list.
* **Implementation Strategy:**
  1. Utilized extended sequence unpacking (`first, *middle, last = items`) to separate the head, internal sequence, and tail into isolated variables.
  2. Reconstructed and returned a new list with positions swapped: `[last, *middle, first]`.
* **Example Output:** `swap_bookends([1, 2, 3, 4, 5, 6])` $\rightarrow$ `[6, 2, 3, 4, 5, 1]`

---

## IV. Constraints & Requirements
* **No Control Flow / Loops:** All logic is executed using direct expression evaluation, string methods, slicing, and sequence unpacking.

---

## V. How to Run
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/moriaean/ECE2112_PA1.git
