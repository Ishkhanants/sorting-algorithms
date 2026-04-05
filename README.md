<div align="center">

```
                                        ╔══════════════════════════════════════════════════╗
                                        ║                                                  ║
                                        ║    ███████╗ ██████╗ ██████╗ ████████╗███████╗    ║
                                        ║    ██╔════╝██╔═══██╗██╔══██╗╚══██╔══╝██╔════╝    ║
                                        ║    ███████╗██║   ██║██████╔╝   ██║   ███████╗    ║
                                        ║    ╚════██║██║   ██║██╔══██╗   ██║   ╚════██║    ║
                                        ║    ███████║╚██████╔╝██║  ██║   ██║   ███████║    ║
                                        ║    ╚══════╝ ╚═════╝ ╚═╝  ╚═╝   ╚═╝   ╚══════╝    ║
                                        ║                                                  ║
                                        ║     A L G O R I T H M S  ·  I N  ·  J A V A      ║
                                        ║                                                  ║
                                        ╚══════════════════════════════════════════════════╝
```

**30 sorting algorithms** — from textbook classics to delightful curiosities —  
each with a clean Java implementation and detailed explanation.

[![Java](https://img.shields.io/badge/Language-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)](https://www.java.com)
[![Algorithms](https://img.shields.io/badge/Algorithms-30-4CAF50?style=flat-square)](#-algorithms-at-a-glance)
[![IntelliJ IDEA](https://img.shields.io/badge/IDE-IntelliJ_IDEA-000000?style=flat-square&logo=intellij-idea)](https://www.jetbrains.com/idea/)

</div>

---

## 🗂 Repository Structure

Every algorithm lives in its own package under `src/`, following a consistent layout:

```
src/
├── bubble/
│   ├── ordinary/
│   │   ├── BubbleSort.java       ← implementation
│   │   └── info.md               ← explanation + complexity analysis

```

---

## ⚡ Algorithms at a Glance

### 🏛 The Classics

| Algorithm | Best | Average | Worst | Space | Stable |
|-----------|------|---------|-------|-------|--------|
| [Bubble Sort](src/bubble/ordinary/) | O(n) | O(n²) | O(n²) | O(1) | ✅ |
| [Recursive Bubble Sort](src/bubble/recursive/) | O(n) | O(n²) | O(n²) | O(n) | ✅ |
| [Selection Sort](src/selection/) | O(n²) | O(n²) | O(n²) | O(1) | ❌ |
| [Insertion Sort](src/insertion/ordinary/) | O(n) | O(n²) | O(n²) | O(1) | ✅ |
| [Binary Insertion Sort](src/insertion/binary/) | O(n log n) | O(n²) | O(n²) | O(1) | ✅ |
| [Recursive Insertion Sort](src/insertion/recursive/) | O(n) | O(n²) | O(n²) | O(n) | ✅ |
| [Merge Sort](src/merge/recursive/) | O(n log n) | O(n log n) | O(n log n) | O(n) | ✅ |
| [Iterative Merge Sort](src/merge/iterative/) | O(n log n) | O(n log n) | O(n log n) | O(n) | ✅ |
| [Quick Sort](src/quick/recursive/) | O(n log n) | O(n log n) | O(n²) | O(log n) | ❌ |
| [Iterative Quick Sort](src/quick/iterative/) | O(n log n) | O(n log n) | O(n²) | O(n) | ❌ |
| [Heap Sort](src/heap/) | O(n log n) | O(n log n) | O(n log n) | O(1) | ❌ |
| [Shell Sort](src/shell/) | O(n log n) | O(n log²n) | O(n log²n) | O(1) | ❌ |

### 🔢 Non-Comparison Sorts

| Algorithm | Best | Average | Worst | Space | Stable |
|-----------|------|---------|-------|-------|--------|
| [Counting Sort](src/counting/) | O(n+k) | O(n+k) | O(n+k) | O(k) | ✅ |
| [Radix Sort](src/radix/) | O(nk) | O(nk) | O(nk) | O(n+k) | ✅ |
| [Bucket Sort](src/bucket/) | O(n+k) | O(n+k) | O(n²) | O(n) | ✅ |
| [Pigeonhole Sort](src/pigeonhole/) | O(n+k) | O(n+k) | O(n+k) | O(k) | ✅ |
| [Bead Sort](src/bead/) | O(n) | O(√n) | O(n²) | O(n²) | ✅ |

### 🌳 Tree-Based Sorts

| Algorithm | Best | Average | Worst | Space | Stable |
|-----------|------|---------|-------|-------|--------|
| [Tree Sort](src/tree/ordinary/) | O(n log n) | O(n log n) | O(n²) | O(n) | ✅ |
| [Cartesian Tree Sort](src/tree/cartesian/) | O(n) | O(n log n) | O(n log n) | O(n) | ❌ |

### 🧩 Hybrid & Advanced

| Algorithm | Description |
|-----------|-------------|
| [Tim Sort](src/tim/) | Merge Sort + Insertion Sort hybrid. Used in Java's `Arrays.sort()` |
| [Intro Sort](src/intro/) | Quick Sort + Heap Sort + Insertion Sort hybrid. Used in C++ STL |
| [Patience Sort](src/patience/) | Based on the card game; finds the longest increasing subsequence |

### 🎭 Quirky & Specialized

| Algorithm | Fun Fact |
|-----------|----------|
| [Cocktail Sort](src/cocktail/) | Bidirectional bubble sort — it sloshes back and forth |
| [Comb Sort](src/comb/) | Bubble sort with a shrinking gap, inspired by broom physics |
| [Gnome Sort](src/gnome/) | Like insertion sort, but a garden gnome is doing it |
| [Cycle Sort](src/cycle/) | Minimizes memory writes — useful for flash storage |
| [Strand Sort](src/strand/) | Pulls sorted strands out and merges them |
| [Pancake Sort](src/pancake/) | Only operation allowed: flip a prefix of the array |
| [Sleep Sort](src/sleep/) | Spawns a thread per element; each sleeps for its own value |
| [Stooge Sort](src/stooge/) | Famously inefficient. O(n^2.7). Don't use in production. |
| [Permutation Sort](src/permutation/) | Tries every permutation until sorted. O((n+1)!) 😱 |
| [Brick Sort](src/brick/) | Also called Odd-Even Sort; parallel-friendly bubble sort |
| [Bitonic Sort](src/bitonic/) | Designed for parallel hardware; works on power-of-2 arrays |
| [Tag Sort](src/tag/) | Sorts by creating an auxiliary tag array — preserves original |

### 🔍 Graph Traversal (Bonus)
| Algorithm | Description |
|-----------|-------------|
| [Breadth-First Search](src/breadthfirst/) | BFS traversal on an adjacency-list graph |

---

## 🚀 Getting Started

### Prerequisites

- **Java 8+**
- **IntelliJ IDEA** (recommended — a `.idea/` project is included) or any Java IDE

### Clone & Run

```bash
git clone https://github.com/your-username/sorting-algorithms.git
cd sorting-algorithms
```

Open the project in IntelliJ IDEA and run any class that contains a `main` method, or compile from the command line:

```bash
# Compile a specific algorithm (example: Merge Sort)
javac src/merge/recursive/MergeSort.java

# Run it
java -cp src merge.recursive.MergeSort
```

---

## 📖 Deep Dives

Each algorithm directory contains an `info.md` with:

- 📝 Plain-English explanation of how it works
- 🔢 Step-by-step worked example
- 📊 Time & space complexity analysis (best / average / worst)
- 🖼 Diagrams illustrating the algorithm's behaviour
- 💡 Notes on stability, in-place behaviour, and real-world use cases

---

## 🧠 Choosing the Right Algorithm

```
Is your data nearly sorted?
├─ Yes → Insertion Sort or Timsort
└─ No
   ├─ Are values integers in a known range?
   │   ├─ Yes → Counting Sort, Radix Sort, or Bucket Sort
   │   └─ No
   │       ├─ Need stable sort?
   │       │   ├─ Yes → Merge Sort or Timsort
   │       │   └─ No  → Quick Sort or Heap Sort
   └─ Is minimising writes critical (e.g. flash memory)?
       └─ Yes → Cycle Sort
```

**General rule of thumb:**

| Scenario | Recommended |
|----------|-------------|
| Small arrays (n < 20) | Insertion Sort |
| General-purpose | Quick Sort / Timsort |
| Guaranteed O(n log n) | Merge Sort or Heap Sort |
| Integer keys, bounded range | Counting / Radix Sort |
| Educational / visualisation | Bubble, Selection, Gnome |
| Parallel hardware | Bitonic Sort, Brick Sort |

---

## 📁 Full Directory Index

<details>
<summary>Click to expand the complete file tree</summary>

```
src/
├── bead/             BeadSort.java
├── bitonic/          BitonicSort.java
├── breadthfirst/     Graph.java
├── brick/            BrickSort.java
├── bubble/
│   ├── ordinary/     BubbleSort.java
│   └── recursive/    RecursiveBubbleSort.java
├── bucket/           BucketSort.java
├── cocktail/         CocktailSort.java
├── comb/             CombSort.java
├── counting/         CountingSort.java
├── cycle/            CycleSort.java
├── gnome/            GnomeSort.java
├── heap/             HeapSort.java
├── insertion/
│   ├── binary/       BinaryInsertionSort.java
│   ├── ordinary/     InsertionSort.java
│   └── recursive/    RecursiveInsertionSort.java
├── intro/            IntroSort.java
├── merge/
│   ├── iterative/    IterativeMergeSort.java
│   └── recursive/    MergeSort.java
├── pancake/          PancakeSort.java
├── patience/         PatienceSort.java
├── permutation/      PermutationSort.java
├── pigeonhole/       PigeonholeSort.java
├── quick/
│   ├── iterative/    IterativeQuickSort.java
│   └── recursive/    QuickSort.java
├── radix/            RadixSort.java
├── selection/        SelectionSort.java
├── shell/            ShellSort.java
├── sleep/            SleepSort.java
├── stooge/           StoogeSort.java
├── strand/           StrandSort.java
├── tag/              TagSort.java  ·  Person.java
├── tim/              TimSort.java
└── tree/
    ├── cartesian/    CartesianTreeSort.java
    └── ordinary/     TreeSort.java
```

</details>

<div align="center">

Made with ☕ and a love for algorithms.

*"An algorithm must be seen to be believed."* — Donald Knuth

</div>
