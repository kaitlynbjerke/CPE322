# Lab 1 - GHDL and GTKWave
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:**
In this lab, we were tasked with downloading GHDL and GTKWave, and analyzing the behavior of different circuit element.

For this lab, I decided to run the **half adder** and **multiplexer** examples.

**Resources Used:** [dsd GitHub](https://github.com/kevinwlu/dsd/tree/master/ghdl), [GHDL/GTKWave Tutorial](https://www.youtube.com/watch?v=H2GyAIYwZbw)

**Process:**
1. Download Notepad++
2. Download GHDL and GTKWave
3. Change the Path Environment Variable to include GHDL and GTKWave bins
4. Copy the code into Notepad, also copy in the test bench code
5. Open the Command Prompt, change directory to the folder with the code
6. Utilize the Command Prompt to do the following:
- Check for syntax errors
- Analyze the code
- Elaborate (build executable)
- Run the code
8. Test that the code works --> View inputs/outputs in GTKWave

Half Adder
---
**Main Code:**

![Main Code](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-05%20173131.png)

**Test Code:**

![Test Code](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-05%20173123.png)

**Wave Output:**

![GTKWave](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-05%20173107.png)

**Behavior of a Half Adder:**
Half adders simply add the bits inputted (A and B).
- The sum equals 1 if either A or B equal 1, but not both (XOR)
- The carry-out equals 1 if *BOTH* A and B equal 1 (AND)
