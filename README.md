# Quantum-Cryptography

The goal of quantum cryptography is to make it possible for two users to communicate in a way that is more secure than the guarantees provided by conventional encryption. In the past, cryptographic security was based on mathematics and took into consideration our current, limited capacity for calculation.The most recent innovation that appears to ensure privacy even when assuming eavesdroppers with infinite processing capacity is quantum cryptography, which employs photons and depends on the principles of quantum physics instead of "extremely large numbers."

Stephen Weisner initially put out the idea of quantum cryptography in his early 1970s paper "Conjugate Coding". Two scientists, Bennet and Brassard, who were familiar with Weisner's theories, were prepared to submit their own ideas by the time the proposal was published in Sigact News in 1983. They created the "BB84," the first quantum cryptography protocol, in 1984. Based on this, the first experimental prototype was created in 1991. It worked across a 32-centimeter range. The technology has improved through time, and the distance has grown to km.

> **State Vectors:** For n qubits, there are $2^n$ possible outcomes, and we can store these amplitudes in lists of length which we call vectors. Since these vectors describe the state of our qubits, we call them “state vectors”.

> **Superpostition:** This is a quantum property that enables qubits to exist in multiple states at the same time. In quantum computing, superposition is used to perform calculations on multiple possible states simultaneously.

> **Entanglement:** Entanglement is a phenomenon where two or more qubits become correlated in such a way that the state of one qubit is dependent on the state of another, even if they are physically separated. Entanglement is a crucial aspect of quantum computing, as it allows qubits to be interconnected in ways that classical bits cannot.

> **Quantum gates:** Quantum gates are the equivalent of classical logic gates in quantum computing. They manipulate qubits, transforming their states based on quantum principles. Quantum gates are used to perform quantum operations on qubits, such as creating superpositions and entanglement.

> **Quantum Circuits:** Quantum computations are represented as sequences of quantum gates, forming quantum circuits. These circuits describe the manipulation of qubits to perform specific tasks, similar to how classical algorithms are composed of logical operations.

## How classical bits are different from qubits?

Classical bits and qubits are fundamental units of information, but they differ significantly in terms of their properties and behavior, primarily due to the principles of classical and quantum mechanics. 

| Classical bits | Quantum bits (qubits) |
| ----------- | ----------- |
| The basic unit of classical information can take one of two possible values: 0 or 1.  It's commonly represented using electrical or physical states like voltage levels, magnetic orientations, or on/off states in a computer.           | The basic unit of quantum information can exist in a superposition of states, which means it can represent 0, 1, or any combination of these states simultaneously.      |
| Classical bits are independent of each other. The value of one bit doesn't affect the value of another bit.          | Qubits can be entangled with each other. Entanglement is a quantum phenomenon where the states of two or more qubits become correlated in such a way that the state of one qubit cannot be described independently of the state of the other qubits.           |
| Measuring a classical bit in a well-defined state (0 or 1) doesn't change its value.           | Measuring a qubit collapses its superposition state into one of the basis states (0 or 1) with probabilities determined by the coefficients in its superposition. This collapse is a fundamental aspect of quantum mechanics and can't be predicted precisely beforehand.         |
| Classical bits are manipulated using classical logic gates (AND, OR, NOT, etc.) in classical computers.    | Qubits are manipulated using quantum gates, which operate on the qubits' superposition states. Quantum computers can use these gates to perform certain calculations more efficiently than classical computers for specific problems.  |
| Classical bits are stable and don't spontaneously change their values due to external factors.  | Qubits are susceptible to noise and decoherence from their environment, causing them to lose their delicate quantum properties and become more like classical bits. This is a significant challenge in building and maintaining stable quantum systems.  |

## Qubits Representation

**Dirac notation:** Dirac notation is a standard mathematical notation used to represent quantum states, operators, and measurements. In this notation, a quantum state (ket) is represented as |ψ⟩, and its complex conjugate is called a bra, represented as ⟨ψ|. For example, the notation |0⟩ represents the quantum state of a qubit in the "0" state.

**Quantum State Vector:** Quantum states are often represented using state vectors in a complex vector space. For a single qubit, the state vector |ψ⟩ can be written as a linear combination of basis states:

  |ψ⟩ = α|0⟩ + β|1⟩

Here, α and β are complex probability amplitudes, and |0⟩ and |1⟩ are the basis states representing the "0" and "1" states of the qubit.

**CNOT Gate:** The CNOT gate works on two qubits: qubit A, which is referred to as the control qubit,
and qubit B, which is the target qubit. On application of a CNOT gate, the control qubit
state remains unchanged. The target qubit state is flipped in case the control qubit is in
state ∣1⟩.

![Image](https://github.com/AniketP04/Quantum-Cryptography/blob/main/assets/CNOT.png)



