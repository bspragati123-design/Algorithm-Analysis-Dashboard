# Algorithm-Analysis-Dashboard

Sorting Analyzer Pro 📊
Empirical Time Complexity Benchmarking Dashboard
Sorting Analyzer Pro is a sleek, client-side web application built for Analysis and Design of Algorithms (ADA) benchmarking. It provides a real-time empirical analysis comparing the practical performance of Bubble Sort (O(n 
2
 )) against Merge Sort (O(nlogn)) across varying array sizes.

🚀 Features
Dynamic Test Bench Configuration: Input custom array sizes (n) via a comma-separated list to instantly benchmark scaling differences.

High-Precision Metrics: Utilizes the JavaScript performance.now() API to log execution time down to a fraction of a millisecond.

Adaptive Micro-Benchmarking Loop: For small array dimensions (e.g., n≤20), the engine automatically scales iterations up to 2,000 runs. It then averages the time to smooth out CPU caching distortions and bypass sub-millisecond precision limitations.

Performance Delta Engine: Dynamically calculates and displays exactly how many times faster Merge Sort performs compared to Bubble Sort for any given input size.

Asynchronous Processing: Leverages a Promise chaining architectural queue to keep the modern dark-themed user interface responsive during heavy computational sorting matrices.

🛠️ Tech Stack & Architecture
Frontend: Pure HTML5 & Semantic markup.

Styling: Modern CSS3 featuring a custom dark mode palette constructed via CSS variables, flexbox/grid structural components, and responsive design paradigms.

Core Engine: Native JavaScript (ES6+), leveraging Int32Array allocations for memory-optimized numeric tracking.

Algorithm Implementations Inside
Bubble Sort: Enhanced with a swapped flag optimization short-circuit, yielding a best-case time complexity of Ω(n) and worst/average case of O(n 
2
 ).

Merge Sort: A structural Divide-and-Conquer algorithm guaranteeing a stable worst, best, and average-case performance profile of O(nlogn).

📈 Performance Benchmarking Context
As you scale your input array size (n), the console logs the widening architectural gap between polynomial growth and linearithmic growth:

Array Dimension (n)	Bubble Sort Complexity	Merge Sort Complexity	Theoretical Efficiency Winner
Small Inputs (n<50)	O(n 
2
 )	O(nlogn)	Comparable due to low overhead
Large Inputs (n>1000)	O(n 
2
 ) (Explosive growth)	O(nlogn) (Logarithmic scaling)	Merge Sort (By orders of magnitude)
🏁 Getting Started
Because this application relies entirely on modern client-side APIs, there are no dependencies to install.

Clone this repository to your local directory:

Bash
git clone https://github.com/YOUR_USERNAME/sorting-analyzer-pro.git
Open the index.html file in any modern web browser (Chrome, Edge, Firefox, Safari).

Type your desired sample sizes into the input array field, and hit Run Benchmark Matrix.

📝 Academic Notes
This mini-project demonstrates the practical divergence between theoretical Big-O notation and hardware execution realities. While Bubble Sort suffers dramatically under large constraints due to excessive memory swaps, Merge Sort maintains balanced performance curves at the cost of O(n) auxiliary space complexity.
