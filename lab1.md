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

**Wave Interpretation:** As seen in the generated wave, the code performs as it should.
- When A=B=0, the sum equals 0 and the carry-out equals 0
- When A=1 and B=0, the sum equals 1 and the carry-out equals 0
- When A=0 and B=1, the sum equals 1 and the carry-out equals 0
- When A=B=1, the sum equals 0 and the carry-out equals 1

Multiplexer
---
**Main Code:**

![Main Code](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-06%20140003.png)

**Test Code:**

![Test Code](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-06%20140206.png)

**Wave Output:**

![GTKWave1](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-06%20103928.png)
![GTKWave2](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-06%20103918.png)
![GTKWave3](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-06%20103906.png)
![GTKWave4](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-06%20103856.png)

**Behavior of a Multiplexer**
- Multiple input signals are sent into the multiplexer (in this case, 4 signals)
- Separate control signals determine which input is sent through to the output
- Only one input signals gets sent through to the output (4:1 MUX)

**Explanation of Binary**
- Two bits of binary can result in four distinct numbers
- 00 = 0, 01 = 1, 10 = 2, 11 = 3

**Wave Interpretation**
- When s0=s1=0, the first input is sent through to the output (a=1), as indicated by the high signal
- When s0=1 and s1=0, the second input is sent through to the output (b=0), as indicated by the low signal
- When s0=0 and s1=1, the third input is sent through to the output (c=1), as indicated by the high signal
- When s0=s1=1, the fourth input is sent through to the output (d=0), as indicated by the low signal

Command Prompt
---
![Command Prompt](https://github.com/kaitlynbjerke/Images/blob/main/Screenshot%202025-02-05%20173155.png)
*Note: These commands are for the half adder example, however the same commands were also used for multiplexer*

- Before these commands, I also changed directory to the folder of my code files.
- The beginning prompts are meant to check the syntax of my code, analyze it, create executable files, and run it.
- Additionally, I created a dumpfile (ha.vcd), and ran it in GTKWave. This created the plots, as shown above.
