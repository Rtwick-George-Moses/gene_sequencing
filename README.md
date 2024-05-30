# gene_sequencing

1. Sequence Differentiation:

Goal: Differentiate two DNA sequences (s1 and s2) to a minimal combined length.
Method:
Assign numerical values to DNA bases:
T: 1
A: -2
G: 3
C: -4
Subtract the corresponding values for each base position between s1 and s2.
2. Subsequence Matching:

Goal: Identify potential matching subsequences between the differentiated sequences.
Method:
Compare the differentiated sequences.
If a section in both sequences has the same value, it might be a matching subsequence.
However, verify the actual base sequence for confirmation (e.g., s1[4:10] and s2[0:6] might have the same differentiated value but not be identical base sequences).
3. Finding All Potential Subsequences:

Goal: Identify all possible matching subsequences of any length (from 1 to n).
Method:
Iterate through all possible starting positions in both sequences.
Store potential subsequences as tuples containing:
(x, y, diff)
x: Start position on s1
y: Start position on s2
diff: Difference value (length of the subsequence + 1)
Append these tuples to a dictionary.
Sort the dictionary in descending order of subsequence length (diff).
4. Building the Alignment (Work in Progress):

Goal: Combine the identified subsequences into a final alignment while considering compatibility with all other subsequences.
(Details of this step are not provided in the code snippet)
5. Scoring (Work in Progress):

Goal: Assign a score to the final alignment based on its quality, potentially considering factors like:
Number of matching bases
Number of mismatches or gaps
Length of the alignment
Note: This explanation is based on the code comments and might require further clarification for the specific application.




share


more_vert






