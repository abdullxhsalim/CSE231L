# ***Objective:***

* Studying AND, OR, NOT, NAND, NOR and XOR logic gates.  
* Learn about how logic diagrams, truth tables, and Boolean algebra are used to express Boolean functions.  
* Prove the extension of inputs of AND and OR gates using the associative law.  
* Utilizing the associative law, and demonstrating the expansion of AND and OR gates' inputs.  
* Get acquainted with circuits utilizing combinational logic.


# ***Theory:***

* #### Logic Gate

A logic gate is an electronic component that takes one or more inputs and produces an output based on a specific rule. These gates are the building blocks of digital circuits. There are different types of logic gates:

\- AND gate: Output is  true (1) only if all inputs are true (1).  
\- OR gate: Outputs true (1) if at least one input is true (1).  
\- NAND gate: Outputs the opposite of an AND gate, true (1) unless all inputs are true (1).  
\- NOR gate: Outputs the opposite of an OR gate, true (1) only if all inputs are false (0).  
\- XOR gate: Outputs true (1) if only an odd number of inputs are true (1).

* #### Truth Table

A truth table is a table that shows all possible input combinations for a gate or circuit and the corresponding output. It helps us to easily see how logic gates work and predict their behavior. We will use truth tables to check how different gates respond to inputs and ensure that the circuits are designed correctly.  
Example: Here’s the truth table for 2-input AND Gate

| Input |  | Output |
| :---: | :---: | :---: |
| **A** | **B** | **F \= (A . B)** |
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

				Table 1: Truth Table of 2-input AND Gate

* #### Boolean Algebra

Boolean algebra is a mathematical way to represent logic operations. It uses symbols and rules to simplify complex logic expressions, making it easier to design circuits. Boolean algebra is necessary because it allows us to reduce the number of gates and make circuits more efficient.  
Example: Let’s consider the Boolean expression, F \= A ⋅ (A \+ B)

We can simplify this expression using Boolean algebra rules:

1. Apply the **Absorption Law**: A ⋅ (A \+ B) \= AA \+ AB \= A \+ AB \= A . (1 \+ B) \= A  
   * This simplification tells us that if A is true, the entire expression will be true regardless of B.

So, the simplified Boolean expression is: F \= A

This reduces the complexity of the circuit, as fewer logic gates are needed to implement this expression.

* #### Combinational Logic

Combinational logic refers to circuits where the output depends only on the current inputs. It doesn't rely on past inputs or states, meaning the output changes instantly when the input changes.   
Example: A half adder is a simple combinational logic circuit that adds two single-bit binary numbers.

* #### Integrated Circuit (IC)

Integrated circuits (ICs) are small electronic devices that contain multiple logic gates packed into one tiny chip. They are used in almost every electronic device to perform different functions using combinational logic.  
Example: The IC 7400 is a quadruple 2-input NAND gate IC. It contains four independent NAND gates, each with two inputs and one output.

Together, these concepts form the foundation for designing and building digital systems like computers, calculators, and other devices.

# ***Apparatus List:***

| No. | Component | Qty |
| :---- | :---- | :---- |
| **1** | IC 7400 Quadruple 2-input NAND gates | 1 |
| **2** | IC 7402 Quadruple 2-input NOR gates | 1 |
| **3** | IC 7404 Hex Inverters (NOT gates) | 1 |
| **4** | IC 7408 Quadruple 2-input AND gates | 1 |
| **5** | IC 7432 Quadruple 2-input OR gates | 1 |
| **6** | IC 7486 Quadruple 2-input XOR gates | 1 |
| **7** | Trainer Board | 1 |
| **8** | Jumper wire | 15 |

 Table 2: Apparatus List

# ***Circuit Diagrams:***

### Experiment \- 1 ![][image1]![][image2]![][image3]

 Fig A: AND Gate             Fig B: OR Gate                Fig C: NOT Gate  

### ![][image4]![][image5]![][image6]

           Fig D: NAND Gate             Fig E: XOR Gate     		Fig F: NOR Gate

### Experiment \- 2

![][image7]  
Fig G: Circuit Diagram of F \= (A . B) . C		Fig H: Circuit Diagram of F \= (A \+ B) \+ C

### Experiment \- 3

![][image8]  
			Fig I: Circuit Diagram of F \= A′ . C \+ A . B′ \+ B . C 

# ***Data Tables:***

### Experiment \- 1

| Input |  | ANDF \= A . B | OR F \= A \+ B | NAND F \= (A . B)′ | NOR F \= (A \+ B)′ | XORF \= (A ⊕ B) |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **A** | **B** |  |  |  |  |  |
| 0 | 0 | 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 1 | 0 | 0 | 0 |

Table 3: Truth Table of 2-input AND, OR, NAND, NOR and XOR Gates

| Input | NOT F \= A′ |
| :---: | :---: |
| **A** |  |
| 0 | 1 |
| 1 | 0 |

Table 4: Truth Table of NOT Gate

### Experiment \- 2

| A | B | C | F \= A . B . C | F \= A \+ B \+ C |
| :---: | :---: | :---: | :---: | :---: |
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 | 1 |
| 0 | 1 | 0 | 0 | 1 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 0 | 1 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

Table 5: Truth Table of 3-input NAND and NOR Gates

| F \= A . B. C \= (A . B) . C |
| :---- |
| F \= A \+ B \+ C \= (A \+ B) \+ C |

     Table 6: Associative Law

### Experiment \- 3

| A | B | C | I1 \= A′ . C | I2 \= A . B′ | I3 \= B . C | F \= I1 \+ I2 \+ I3 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 | 0 | 1 |
| 0 | 1 | 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 0 | 1 | 0 | 1 |
| 1 | 0 | 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 0 | 0 | 0 |
| 1 | 1 | 1 | 0 | 0 | 1 | 1 |

Table 7: Truth Table of F \= A′ . C \+ A . B′ \+ B . C

# ***Questions and Answers:***

### Q1. Is it possible to make a 3-input NAND or NOR gate with 2-input NAND or NOR gates? Justify your answer.

Answer:  
Yes, it is possible to make a 3-input NAND or NOR gate with 2-input NAND or NOR gates.

#### Making a 3-input NAND gate with 2-input NAND gates:

The 3-input NAND gate function is: NAND(A, B, C) \= (A . B . C)′

Here's how to construct it using only 2-input NAND gates:

1. **Compute (A . B)′:**  
   I1 \= NAND(A, B) \= (A . B)′  
2. **Use 2-input NAND Gate to invert I1**:

I2 \= NAND(I1, I1)	 \= NAND((A . B)′, (A . B)′) 

\= ((A . B)′ . (A . B)′)′ 

\= ((A . B)′)′ \[Idempotent Law\]

\= A . B \[Negation Law\]

3. **Use 2-input NAND Gate to compute (A . B . C)**′:

F \= NAND(I2, C) 	\= NAND((A . B), C) 

\= ((A . B) . C)′ 

\= (A . B . C)′ \[Associative Law\]

#### Making a 3-input NOR Gate with 2-input NOR gates:

The 3-input NOR gate function is: NOR (A, B, C) \= (A \+ B \+ C)′

Here's how to construct it using only 2-input NOR gates:

1. **Compute (A \+ B)′:**  
   I1 \= NOR (A, B) \= (A \+ B)′  
* **Use 2-input NOR Gate to invert I1**:

I2 \= NOR(I1, I1)		 \= NOR((A \+ B)′, (A \+ B)′) 

\= ((A \+ B)′ \+ (A \+ B)′)′ 

\= ((A \+ B)′)′ \[Idempotent Law\]

\= A \+ B \[Negation Law\]

* **Use 2-input NOR Gate to compute (A \+ B \+ C)′:**

F \= NOR(I2, C) 	\= NOR((A \+ B), C) 

\= ((A \+ B) \+ C)′ 

\= (A \+ B \+ C)′ \[Associative Law\]

# ***Discussion:***

We studied how to use different logic gates: AND, OR, NAND, NOR, and XOR. These gates help in creating conditions for making decisions in electronics. In our experiments, we found that the results from both the tests and real-world usage matched exactly.

### Here’s what we learned from each experiment:

#### **Experiment 1**: Basic operations

We explored how the basic logic gates work, like AND, OR, and others. We saw how each gate produces a certain output depending on the inputs it receives.

#### **Experiment 2**: Associative Law

This experiment showed that the grouping of operations doesn’t change the result. For example, in an AND operation, grouping (A AND B) AND C gives the same result as A AND (B AND C).

#### **Experiment 3**: Boolean Functions

 We learned how to use combinations of logic gates to represent complex Boolean functions. These functions are used to solve real-world problems in electronics and computing.

This helped us understand how logical operations can be used to perform tasks efficiently.

### Precautions

- Check for faulty wires before the experiment to ensure proper connection  
- Use an IC Remover so that the IC pins don’t become damaged.  
-  Ensure proper connection of input and output pins: Always apply input voltages only to designated input pins and measure/output signals only from designated output pins. Incorrect connections may damage the circuit components or produce erroneous results.

# ***Simulation**:*

Simulation for the Boolean Expression F \= A′ . C \+ A . B′ \+ B . C  
![][image9]  
	Fig J: Simulation for the Boolean Expression F \= A′ . C \+ A . B′ \+ B . C 
