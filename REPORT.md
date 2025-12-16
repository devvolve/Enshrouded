REPORT – The Triad’s Feast
Overview
This document describes the primary development challenges encountered during the creation of The Triad’s Feast and the solutions implemented by the team.

---

Angie’s Challenges
Learning Unreal Engine from Scratch
Challenge:
With no prior experience in Unreal Engine, understanding the engine’s structure, Blueprints, and file workflows felt overwhelming.

Fix:
Researched beginner UE5 tutorials
Broke down tasks into smaller components
Practiced building simple systems before integrating them into the main level

---

Creating the Inventory System
Challenge:
The inventory system required many interconnected files and Blueprint references.
One missing variable or broken reference caused the entire system to fail.

Fix:
Followed tutorials step-by-step
Used Blueprint debugging tools to track function failures
Rebuilt components systematically ensuring all references were valid
Documented each function to avoid future breakage

---

Navigating GitHub Version Control
Challenge:
Accidentally deleted major files from the repo, nearly causing project failure.
Unfamiliarity with cloning, pushing, and pulling made collaboration difficult.

Fix:
Watched Git/GitHub Crash Course tutorials
Learned proper workflow:
clone → branch → commit → push → pull request
Coordinated with teammate to prevent merge conflicts
Enabled Git LFS for large assets (optional improvement)

---

Daniyal’s Challenges
AI Shadows & Behavior Logic
Challenge:
Implementing shadow entities that respond to light, darkness, and the sanity meter required multiple overlapping Blueprint systems.
AI sometimes froze or ignored the player.

Fix:
Re-structured Behavior Trees
Adjusted navmesh boundaries
Ensured BlackBoard keys updated correctly
Added timers to prevent AI state-locking

---

Light/Darkness & Enshroud Meter
Challenge:
Balancing visibility, fear, and enemy spawn triggers required precise tuning.
Darkness volumes sometimes overlapped incorrectly.

Fix:
Created modular darkness volumes
Implemented sanity decay functions tied to line traces and lighting checks
Used debug drawing to visualize detection logic

---

Puzzle Integration
Challenge:
Lighting and electrical puzzles broke when integrated with the main level.

Fix:
Rebuilt puzzle logic inside child Blueprints
Standardized interaction event names
Re-tested puzzles using the final player pawn to ensure compatibility

---

Summary
The development of The Triad’s Feast required learning a complex engine, debugging multi-system interactions, and adapting to version control in a team setting.
Through persistence, debugging, and collaborative problem solving, the team overcame each challenge and successfully delivered a playable psychological horror experience.
