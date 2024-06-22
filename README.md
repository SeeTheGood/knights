# Knights and Knaves Puzzles

This repository contains Python code to solve Knights and Knaves logic puzzles. The puzzles are based on statements made by individuals who are either knights (who always tell the truth) or knaves (who always lie). The goal is to determine the identity of each individual based on their statements.

## File Structure

- `logic01.py`: Contains the logic classes and functions for constructing and evaluating logical sentences.
- `puzzle01.py`: Defines the symbols, statements, and knowledge bases for different puzzles and checks their solutions.

## Logic Module

The logic module (`logic01.py`) includes classes to represent logical symbols, operations, and model checking:

- `Symbol`: Represents a basic logical symbol.
- `Not`: Represents logical negation.
- `And`: Represents logical conjunction.
- `Or`: Represents logical disjunction.
- `Implication`: Represents logical implication.
- `Biconditional`: Represents logical biconditional.
- `model_check`: Function to check if a given knowledge base entails a query.

## Puzzles

### Puzzle 0

- **A** says: "I am both a knight and a knave."
- **Knowledge Base**:
  - A is either a knight or a knave.
  - B is either a knight or a knave.
  - C is either a knight or a knave.
  - A cannot be both a knight and a knave.
  - B cannot be both a knight and a knave.
  - C cannot be both a knight and a knave.
  - A is a knight if and only if A's statement is true.

### Puzzle 1

- **A** says: "We are both knaves."
- **B** says nothing.
- **Knowledge Base**:
  - A is either a knight or a knave.
  - B is either a knight or a knave.
  - C is either a knight or a knave.
  - A cannot be both a knight and a knave.
  - B cannot be both a knight and a knave.
  - C cannot be both a knight and a knave.
  - A is a knight if and only if A's statement is true.

### Puzzle 2

- **A** says: "We are the same kind."
- **B** says: "We are of different kinds."
- **Knowledge Base**:
  - A is either a knight or a knave.
  - B is either a knight or a knave.
  - C is either a knight or a knave.
  - A cannot be both a knight and a knave.
  - B cannot be both a knight and a knave.
  - C cannot be both a knight and a knave.
  - A is a knight if and only if A's statement is true.
  - B is a knight if and only if B's statement is true.

### Puzzle 3

- **A** says either: "I am a knight." or "I am a knave." (but you don't know which).
- **B** says: "A said 'I am a knave'." and "C is a knave."
- **C** says: "A is a knight."
- **Knowledge Base**:
  - A is either a knight or a knave.
  - B is either a knight or a knave.
  - C is either a knight or a knave.
  - A cannot be both a knight and a knave.
  - B cannot be both a knight and a knave.
  - C cannot be both a knight and a knave.
  - A is a knight if and only if A's statement is true.
  - B is a knight if and only if B's statement is true.
  - C is a knight if and only if C's statement is true.

## Running the Code

To run the code and solve the puzzles, execute the following command:

```sh
/usr/local/bin/python3.11 "/path/to/puzzle01.py"

