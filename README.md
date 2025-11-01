# lean4playground

A sandbox repository for experimenting with Lean 4, a theorem prover and functional programming language.

## About

This is a playground repository for exploring various features of Lean 4, including:

- Theorem proving and formal verification
- Functional programming patterns
- Type theory concepts
- Mathematical formalization
- Proof tactics and strategies

## Getting Started

### Prerequisites

- Install Lean 4 from [https://leanprover.github.io/](https://leanprover.github.io/)
- Install VS Code with the Lean 4 extension (recommended)

### Creating a New Lean Project

```bash
# Initialize a new Lean project
lake init <project-name>

# Build the project
lake build
```

## What is Lean 4?

Lean 4 is a functional programming language and theorem prover. It's used for:

- **Formal Mathematics** - Proving mathematical theorems with computer-verified correctness
- **Software Verification** - Proving properties about programs
- **Type Theory** - Exploring dependent type theory and its applications
- **Programming** - Writing efficient, verified functional programs

## Useful Resources

### Official Documentation
- [Lean 4 Manual](https://leanprover.github.io/lean4/doc/)
- [Theorem Proving in Lean 4](https://leanprover.github.io/theorem_proving_in_lean4/)
- [Functional Programming in Lean](https://leanprover.github.io/functional_programming_in_lean/)

### Learning Materials
- [Mathematics in Lean](https://leanprover-community.github.io/mathematics_in_lean/)
- [Lean 4 Metaprogramming Book](https://leanprover-community.github.io/lean4-metaprogramming-book/)
- [Natural Number Game](https://adam.math.hhu.de/#/g/leanprover-community/nng4) - Learn Lean through interactive puzzles

### Community
- [Lean Zulip Chat](https://leanprover.zulipchat.com/)
- [Lean Community](https://leanprover-community.github.io/)

## Example: Hello World in Lean

```lean
def main : IO Unit :=
  IO.println "Hello, Lean 4!"
```

## Example: Simple Theorem

```lean
theorem add_comm (a b : Nat) : a + b = b + a := by
  induction a with
  | zero => simp
  | succ a ih => simp [Nat.add_succ, ih]
```

## Use Cases

- Mathematical research and formalization
- Learning formal methods and proof techniques
- Exploring type theory and dependent types
- Building verified software
- Experimenting with metaprogramming

## Next Steps

Start experimenting with Lean 4 by:
1. Writing simple functions and testing them
2. Proving basic theorems about natural numbers
3. Exploring the standard library
4. Trying interactive tutorials like the Natural Number Game
5. Reading "Theorem Proving in Lean 4"
