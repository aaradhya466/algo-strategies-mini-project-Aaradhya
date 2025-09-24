## 📊 Final Summary: Algorithmic Strategies Comparison

| Problem               | Strategy           | Time Complexity              | Domain              | Notes |
|------------------------|--------------------|------------------------------|---------------------|-------|
| TV Commercial Scheduling | Greedy (Job Sequencing) | O(n log n) for sorting + O(n) for scheduling | Media & Advertisement | Efficient for maximizing ad revenue in limited slots. |
| Knapsack (Budget Planning) | Dynamic Programming (0/1 Knapsack) | O(n × Capacity) | Budget Planning | Ensures optimal selection of projects/items under budget. |
| Sudoku Solver         | Backtracking       | Exponential (O(9^(n))) in worst case | Gaming / Puzzles | Works well for typical puzzles, but slows down for harder cases; recursion depth matters. |
| Password Cracking     | Brute-Force        | O(|Charset|^L) (exponential) | Cybersecurity | Impractical for large charsets/lengths; demonstrates need for strong passwords. |

## 🔎 Insights: Observed vs. Theoretical Performance

- **TV Commercial Scheduling (Greedy):**  
  Observed performance matches theory — very fast, as sorting dominates.  
  Time grows nearly linearly with ads. Memory usage negligible.

- **Knapsack (DP):**  
  Observed performance grows with number of items × budget capacity.  
  Matches O(n × W).  
  Memory profiling shows DP table dominates space usage.

- **Sudoku Solver (Backtracking):**  
  Observed time increases drastically with puzzle difficulty (more blanks).  
  Matches exponential worst-case analysis.  
  Stack usage noticeable since recursion depth can approach 81.

- **Password Cracking (Brute-Force):**  
  Observed time grows exponentially with password length.  
  Matches theoretical O(|Charset|^L).  
  Even small increases in length or charset size cause time explosion.
