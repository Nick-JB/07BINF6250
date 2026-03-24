# Introduction
Description of the project

# Pseudocode

```
BWT Transformation Function:
    Append '$' to the end of input string
    Initialise a list to store all cyclic rotations
    Loop through every index in the length of the string
      Take a substring from ind to end and concatenate it with substring from start to ind
      Store the rotation along with its index position in the list

    Sort the rotations lexicographically
    Initialise a string to store the transformed string
    Initialise a list for original indices

    Loop through each rotation in the sorted rotations list
      Pick the last character of the rotation
      Append the character to the transformed string
      Store the original index position in the original indices list

  Return transformed string and original indices

Suffix Array Function:
    Append '$' to the end of the string
    Initialise a list called suff
    Loop through every index in the length of the string
      If ind equals 0 (suffix starts at the last position)
        Suff ind becomes length of string - 1
      Else
        Suff ind becomes ind - 1
      Take out the suffix from that position till the end
      Store the suffix along with its starting position
    Sort the suffix list lexicographically
    Extract the starting positions from the sorted list
  Return the starting positions as a list

BWT from suffix array Function:
    Append '$' to the text
    Initialise a string called transform
    Loop through every index in suffix positions
      Pick the character just before the suffix begins (suffix - ind; character - text[ind-1])
      Append the character to transform
  Return the transform

Calculate counts Function:
    Count the frequency of each character using Counter and sort lexicographically
    Initialise the current count as 0
    Loop through each character in the sorted order
      Store the frequency of the character
      Assign current count (number of characters that occurred until then) as the count
      Add the stored frequency to current_count
  Return the count dict

Calculate occurences Function:
    Pick the unique alphabets(characters) from BWT string
    Initialise a 2D array with zeros where rows - alphabets columns - position in BWT string
    Create a mapping from each character to its row index
    Loop through each position and character in BWT string
      Add 1 to all the positions from index onwards in that character row
BWT Transformation Function:
    Append '$' to the end of input string
    Initialise a list to store all cyclic rotations
    Loop through every index in the length of the string
      Take a substring from ind to end and substring from start to end
      Store the rotation along with its index position in the list

  To sort the rotations lexicographically
    Initialise a string to store the transformed string
    Initialise a list for original indices

    Loop through each rotation in the sorted rotations list
      Pick the last character of the rotation
      Append the character to the transformed string
      Store the original index position in original indices list

  Return transformed string and original indices

Suffix Array Function:
    Append '$' to the end of the string
    Initialise a list called suff
    Loop through every index in the length of the string
      If ind equals 0 (suffix starts at the last position)
        Suff ind becomes length of string - 1
      Else
        Suff ind becomes ind - 1
      Take out the suffix from position -1 - ind till the end
      Store the suffix along with its starting position
    Sort the suffix list lexicographically
    Extract the starting positions from the sorted list
  Return the starting positions as a list

BWT from suffix array Function:
    Append '$' to the text
    Initialise a string called transform
    Loop through every ind in suffix positions
      Pick the character just before the suffix begins (suffix - ind; character - text[ind-1])
      Append the character to transform
  Return the transform

Calculate counts Function:
    Count the frequency of each character using Counter and sort lexicographically
    Initialise the current count value as 0
    Loop through each character in the sorted order
      Store the frequency of the character
      Assign current count (number of characters that occurred until then) as the count
      Add the stored frequency to current_count
  Return the count dict

Calculate occurences Function:
    Pick the unique alphabets(characters) from BWT string
    Initialise a 2D array with zeros where rows - alphabets columns - position in BWT string
    Create a mapping from each character to a row index
    Loop through each position and character in BWT string
      Add 1 to all the positions from ind onwards in that row
    Convert the array into a dictionary where each character maps to its list of occurence counts
  Return the sorted dictionary

```

# Successes
Description of the team's learning points

# Struggles
Description of the stumbling blocks the team experienced

# Personal Reflections
## Group Leader
Group leader's reflection on the project

## Other member
Aaronie Jersha Jenyfred: For this project, I feel the conceptual understanding was the hardest part. The overview of pseudocode that was given for eaach function really helped in navigating the algorithmic logic. This project also broadened my understanding of indexing and string operations. Also, debugging and brainstorming together as a group made the work real smooth. 

# Generative AI Appendix
None
