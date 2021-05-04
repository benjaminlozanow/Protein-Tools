# Protein-Tools
Set of functions and functionalities that can help while working with proteins.

## 1-letter code protein sequence

- `mass_calculator(seq, method)`determines the mass of the input sequence *seq* with the average or monoisotopic *method*.  

  Parameters:  
  **seq**: input sequence as a string.  
  **method**: *str {'average', 'monoisotopic'}*  

  Returns:  
  *mass* from input sequence.   

- `aa_distribution(seq)`graphical representation of the distribution of the amino acids presents in the sequence *seq*.  

  Parameters:  
  **seq**: input sequence as a string.  

  Returns:  
  *plot*

- `charge(seq, exclude, polarity)`calculates the maximum charge possible for the input sequence *seq*. Based on the presence of acid (positive) or basic (negative) amino acids in the sequence. For the positive charge the amino acids Arginine (R), Lysine (K) and Histidine (H) were considered. While for the negative charge the amino acids Glutamic Acid (E) and Aspartic Acid (D). Any of these amino acids can be excluded for charge calculation (normally Histidine ('H') is excluded due to is lack of protonation).

  Parameters:  
  **seq**: input sequence as a string.  
  **exclude**: *str {'K', 'R', 'H', 'D', 'E'}*   
  **polarity** = *str {'positive', 'negative'}*  

  Returns:  
  positive and or negative charge (pos, neg)
