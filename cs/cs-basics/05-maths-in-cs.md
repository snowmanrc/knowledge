# Mathematic in CS

Mathematics is the science of logic, shapes, quantities, and arrangement. It provides the rules and structure that keep all software and hardware from collapsing and thus plays an important role in Computer Science.

## Role of Mathematics

### In CS specifically

1. `The Bottom Layer` Used at the hardware level in ALUs to do basic mathematical and logical operations at immense speeds.
2. `The Middle Layer` Used at the OS level to make mathematical rules and algorithms for process scheduling, memory management and file operations.
3. `The Top Layer` Used in applications for algorithms

### In Other Fields

1. Medical devices and Health: Blood pressure tracker, heart beat tracker, eyesight tester and detection of tumors (using AI).
2. Robotics: For robot movement and stability.
3. Engineering: Software to simulate and model real world forces.

## Optimization

The process of determining the absolute best solution out of all possible solutions is called optimization. Basically, it is the process of choosing the best possible inputs and algorithms to get the best possible output.

> [!tip] Mathematical Modelling and Computers
> Any process that can be described with mathematical operations and relations, a computer can model and optimize it.

Real world optimizations fall into two basic categories:
1. *Maximizing* something to get the most of it.
2. *Minimizing* something to get the least of it.

## Function

A function is a mathematical rule that takes an input and returns an output. A mathematical rule is a function as long as:
+ It must work for all input values assigned to it.
+ It must return the same output for the same set of inputs.

> [!note] Functions in CS
> Functions in CS can often be impure functions i.e. they can return different outputs given the same set of inputs.

## Cryptography

Cryptography is the science of locking and securing information so that only the intended recipient can read and process it.
### Encryption

Encryption is the process of converting readable data into unreadable, scrambled data using a mathematical transformation for securing information.

+ *Plain Text* -> Original unscrambled message
+ *Cipher Text* -> Scrambled message after encryption

Encryption maybe of two types depending on the key used for the transformation:
1. *Symmetric Encryption* where both the sender and receiver share the same secret key. It is like having two duplicate keys of the same lock.
2. *Asymmetric Encryption* where the senders have a different key (public key) and the receiver has a different key (private key). Everyone can send the receiver an encrypted message but only the receiver can uncrypt it using the private key.

### Caesar Cipher

It is an example of an encryption technique where the characters are shifted to get a scrambled message and then shifted back to get the real message. It is also called the *Character Shift Cipher*.
$$\text{Ciphertext Letter} = f(\text{Plaintext Letter}) = \text{Plaintext Letter} + \text{Key}$$

## Core CS Math Foundations

### Propositional Logic

Computers make decisions by using logic. *A proposition is a statement that is either true or false and never in-between.*

Decisions are made by operating on these propositions by using the three basic logic operations:
1. **NOT** (Negation) -> Inverts the value.
2. **AND** (Conjunction) -> Only *true* when both inputs are *true*.
3. **OR** (Disjunction)-> *True* when either input is true.

Other than these three basic gates, some other types of logic operations are:

+ **NAND** (NOT-AND / Universal) -> Only *false* when both inputs are *true*
+ **NOR** (NOT-OR) -> Only *true* when both inputs are *false*
+ **XOR** (Exclusive OR) -> Only *true* when both inputs are *different*
+ **XNOR** (Exclusive NOR) -> Only *true* when both inputs are *same*

### Set Theory

*A set is a **well-defined** collection of **distinct** objects.*

Operations include:
1. **Union**
2. **Intersection**
3. **Difference**
4. **Complement**
5. **Subset**
