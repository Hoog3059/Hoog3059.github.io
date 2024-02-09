---
layout: post
title: Solving puzzles using quantum computers
description: Writing a quantum algorithm for solving Battleships puzzles.
img: assets/projects/battleships_grover/thumbnail.png
date: 2024-01-31
importance: 20240131
category: university
---

*By Jan van den Bos, Timo Hoogenbosch and Borislav Semerdzhiev.*

You can read the full research paper [here](/assets/projects/battleships_grover/report.pdf).

Quantum computing can in theory be used to solve NP-hard problems more efficiently than any classical computer possibly can. This paper focuses on implementing the quantum algorithm known as Grover's algorithm to solve the famous puzzle called 'battleships'. Grover's algorithm is implemented by creating a so called oracle function that checks if a trial solution satisfies all criteria of a correct solution. The algorithm was found to be working on a simulator. However, to be able to execute it on a real quantum computer a high quantum volume is needed. At the time of writing this report there is no quantum computer available with the required quantum volume. This problem could be overcome in the future by introducing quantum error correction and/or higher fidelity gates. In order to mitigate the shortcomings of the current available hardware for running simulations, we have additionally introduced a few optimizations that aim to reduce the number of used qubits, and hence, bring forth an exponential speed up.

The data and data analysis code can be found [here](https://deepnote.com/@quantum-engineering-project/Quantum-Engineering-Project-f7dc926d-60cb-4400-9d30-82a530e8805b).