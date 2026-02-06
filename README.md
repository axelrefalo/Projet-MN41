# Truss Structure Equilibrium Analysis

C# program that calculates the equilibrium of a 2D truss structure under applied forces.

**Academic Project - Fall 2020**  
Axel Refalo & Nicolas Meyer - UTBM

## Overview

Analyzes a truss structure (8 nodes, 12 bars) and computes:
- Node displacements
- Support reactions
- Bar tensions (tension/compression)

## Features

- Reads input from `Donnee.txt`
- Three solving methods: LU decomposition, Gauss elimination, Thomas algorithm
- Exports results to `Resultat.txt`
- Automatic validation (force equilibrium check)

## Usage

1. Place `Donnee.txt` in the Debug folder
2. Compile and run the program
3. Check results in `Resultat.txt`

## Input File Format

The `Donnee.txt` file must contain:
- Number of elements and nodes
- Young's modulus and bar diameter
- Node coordinates
- Connection table
- Displacement constraints
- Applied forces
- Solving method (1=LU, 2=Gauss, 3=Thomas)

## Test Cases

1. 5N horizontal force on N3
2. 10N force at 315° on N5
3. 20N vertical force on N4

## Output

- Node displacements (U, V in mm)
- Applied forces (Fx, Fy in N)
- Bar tensions with compression/tension indicator (N)
