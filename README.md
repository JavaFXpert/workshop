## This page is: [qisk.it/gids](http://qisk.it/gids)
## Resources for GIDS Architecture Quantum Computing Workshop:

#### Title: [Quantum Computing Workshop for Classical Developers](https://wurreka.com/ict/virtual-conference/architecture/session/quantum-computing-workshop-for-classical-developers) 

#### Presenter: [James Weaver](https://twitter.com/javafxpert)

- [James Weaver's presentations slides](https://slides.com/javafxpert/qiskitblocks)
  - QiskitBlocks game site [qisk.it/blocks](https://github.com/JavaFXpert/QiskitBlocks)
  - Open-source quantum computing software development framework site [Qiskit.org](http://qiskit.org) 
  - Quantum computing textbook that leverages Qiskit [qisk.it/textbook](http://qisk.it/textbook) 

#### [IBM Quantum Experience](https://quantum-computing.ibm.com/) (where you'll create a quantum game)

#### Quantum Game Challenge (Build a quantum 8-ball)

1. Optional but recommended if you're new to Qiskit:
  - Take the [Create your first quantum circuit](https://quantum-computing.ibm.com/docs/iqx/first-circuit) tutorial (great primer on using Circuit Composer).
  - Take the [Code your first quantum circuit](https://quantum-computing.ibm.com/docs/iql/first-circuit) tutorial  (great primer on using Qiskit Notebooks).
2. In the IBM Quantum Experience Circuit Composer, create a three-wire circuit whose measurements are randomly distributed among 000 - 111.
   - View the **Statevector** and **Measurement Probabilities** from the **Visualizations** tab (bar graph image) on the left side of the page.
   - Observe the results when running your circuit on a backend quantum system or simulator. The shortest queues are typically with the 32 qubit simulator `ibmq_qasm_simulator in ibm-q/open/main`
3. Create the circuit using Python and Qiskit in an IBM Quantum Experience Jupyter notebook.
   - Make the program print out a message unique to each measured state (e.g. state 000 message might be "The quantum 8-ball says it's most likely"). For reference, here are the [possible answers from the original Magic 8-Ball](https://en.wikipedia.org/wiki/Magic_8-Ball#Possible_answers).
   - If you'd like some hints, please see [this partial solution](https://github.com/JavaFXpert/workshop/blob/master/quantum_8ball_hints.ipynb)
   - For reference, here is [one possible solution](https://github.com/JavaFXpert/workshop/blob/master/quantum_8ball_solution.ipynb)
4. If you have time:
   - Rather than using a simulator, use the `from_instruction()` and `sample_counts()` methods of the `qiskit.quantum_info.Statevector` class. Your circuit should not have measure operations. 
   - Expand the circuit to four or five wires.
   - Add various single and multi-qubit gates to the circuit (in the Circuit Composer first if you'd like) and observe their effects on the measurement probabilities and results.
   
<br/>
<a title="ChristianHeldt / Public domain" href="https://commons.wikimedia.org/wiki/File:Magic8ball.jpg"><img width="256" alt="Magic8ball" src="https://upload.wikimedia.org/wikipedia/commons/9/90/Magic8ball.jpg"></a>
