# table-tennis-stroke-serve-ontology
# Table Tennis Notation System (TTNS)
A theoretical framework and symbolic ontology for the formal encoding of table tennis strokes, serves and tactics. This system provides a compact language to describe the game's complexity, linking physics (force, spin, drag) to practice for coaching, player development and AI-assisted analysis.

> **Book Project:** The theoretical foundations and full specification of this system are detailed in the forthcoming book "*Spin, Speed, Strategy - A Mathematical Guide to Table Tennis*", submitted to Springer.

## 🎯 Core Philosophy

The TTNS moves beyond simple outcome-based statistics. It is a minimal, physics-aware language designed to capture the **intention, execution, and interaction** of shots within a rally, treating table tennis as both an art and a science.

## 📘 The Notation Scheme
The system is built on a binary code that describes the physics of the racket-ball interaction, its outcome, and the tactical intention.

1. Fundamental Stroke Parameters
These three binary digits form the core axes of the notation.
A. Force Application Mode: Encodes the nature of the impact.
1 (Direct Force): Kinetic energy is applied through the ball's centre of mass, prioritising translational velocity (speed).
0 (Tangential Force): Kinetic energy is applied tangent to the ball's surface, prioritising angular velocity (spin).
B. Primary Kinetic Outcome: Encodes the dominant ballistic property of the shot.
1 = Speed.
0 = Spin.
C. Tactics Intent: Encodes the dominant characteristic of two opposing tactical categories.
1 = Tactic-1 (Winner Strategy): Aimed to win the point outright.
0 = Tactic-0 (Forcing Error Strategy): Aimed to induce an error from the opponent.

2.Stroke and Serve Intention Tokens
This layer classifies the type of shot played.

1 = Serve
2 = Stroke
A. 2-bit Serves and Strokes

The first digit after the token defines the shot category.

Serves:
1.11: Serve-Short Attack
1.10: Serve-Short Flick
1.01: Serve-Short Push
1.00: Serve-Short Sway

Strokes:

2.11: Attack
2.10: Flick
2.01: Push
2.00: Sway

*( 3-bit and 4-bit Serves and Strokes will be added here on request.)*

3. The DQ4 four-level quantification
A novel parameter that quantifies a discrete attribute across four levels of intensity:

Hit Strength: Quantifies the intensity of direct force:

1/11/111/1111 = Present/Fast/Very/Exceptional

Brush Strength: Quantifies the intensity of tangential force:

0/00/000/0000 = Present/Strong/Very/Exceptional

Tactic-1 Intensity (Winner): Quantifies the commitment to a winning strategy:

1/11/111/1111 = Present /Habitual/Intentional/Exceptional

Tactic-0 Intensity (Force Error): Quantifies the commitment to an error-forcing strategy:

0/00/000/0000 = Present /Habitual/Intentional/Exceptional

4. The ε (epsilon) Strength Factor
A novel, unified parameter that quantifies the strength of any attribute on a 15-level discrete scale.

Definition: ε: = 2i -1, where i is the ith digit in a stroke, serve or tactic code.

Purpose: The ε-factor provides a single, comparable metric to measure the strength of attributes like Hit, Brush, Speed, Spin, Tactic-1 and Tactic-0.

5. The δ (delta) Variation Measure
An operator that quantifies the tactical disruption or change between two consecutive shots.

δ measures the variation in:

*   Speed (δ₁)
*   Spin (δ₀)
*   Placement (δp)
*   Timing (δt)
*   Rhythm (δr)

## 🚀 Applications

This ontology is designed as a foundational tool for:

Coaches: Provides a reproducible, objective framework for technical and tactical feedback, moving beyond subjective description to quantifiable instruction.
Players: Enables structured self-analysis and precise goal setting by offering a clear language to describe technical execution and tactical choices.
Analysts & Scouts: Offers a standardised data ontology for match analysis, performance benchmarking and cross-context player comparison.
AI & Simulation: Serves as a formal grammar for reasoning, predictive modelling, and the development of intelligent training systems and synthetic opponents.

## 📖 How to Use This Repository

This repository contains the complete specification for the Table Tennis Notation System (TTNS). It is intended as a living document for players, coaches, and researchers.

## 🔗License

This work is openly shared under the permissive MIT License, which encourages both academic and commercial use with appropriate attribution.

## 📜 Citation

If you use this framework in your research or project, please use the following citation format:
> *Ji, X. (2025). Spin, Speed, Strategy – A Mathematic Guide to Table Tennis. Manuscript submitted for publication.*
