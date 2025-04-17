# Lab 11 - Qiskit
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** In This lab, I worked with Qiskit, which is a development tool for quantum computing.

Creating an API Token
---
1. Go to the [IBM Quantum Platform](https://quantum.ibm.com/)
2. Create an account
3. Copy the API Token located in the top right corner

![API Token](https://github.com/kaitlynbjerke/Images/blob/main/APIToken.png)

Preliminary Steps
---
- Install software by typing `pip install qiskit` in the terminal
- Additionally, navigate to the lesson 11 folder in the iot GitHub

qiskit_terra_example.py
---
At first, I faced some issues with running this example due to some functions being outdated. However, after altering the code, I was able to successfully run the python script.

![new code](https://github.com/kaitlynbjerke/Images/blob/main/terra_new_code.png)

Output:

![terraOut](https://github.com/kaitlynbjerke/Images/blob/main/qiskit_terra.png)

The output shows the frequency of the possible states of the qubits (or quantum bits). Thus, the number next to the bit stats ('00', '11') shows how many times that state was measured when we sampled.

Other Examples
---
I have attempted other examples, however I still have not gotten them properly working yet.

**magic_square.py:** This code required some alterations. Most notably, I had to change "i" to "id" when calling `qc.i(b)`. This resulted in successful output in the terminal. However, upon examining the code, I believe it draws a quantum circuit based on "Alice's" and "Bob's" input. I am not sure if I am supposed to see output beyond the initial user input.

![magic](https://github.com/kaitlynbjerke/Images/blob/main/magic.png)

**qiskit_aer_example.py:** The Aer code has interesting functionality, as it is meant to simulate a quantum circuit, while implementing noise modeling. As it stands, this code is still largely unfunctional on my device. I have made some alterations based on [this](https://docs.quantum.ibm.com/api/qiskit-ibm-runtime/fake-provider) link to improve the functionality of the code.

My main alternation was changing the line `from qiskit.providers.fake_provider import FakeManilaV2` to `from qiskit_ibm_runtime.fake_provider import FakeManilaV2`. This allows me to get some output from the code, however I still get an error message after the "Ideal: " line.

![aer](https://github.com/kaitlynbjerke/Images/blob/main/aer.png)

The numbers (541, 483) record how often each bitstring ("111", "000") was measured.
