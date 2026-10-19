NOTE: AI was used in Making of Simulation

# 🌿 Calvin-Benson-Bassham (CBB) Cycle Kinetic Simulator

![License: MIT](https://img.shields.io/badge/License-MIT-emerald.svg)
![Biochemistry](https://img.shields.io/badge/Pathway-Calvin--Benson--Bassham-06b6d4.svg)
![Deploy](https://img.shields.io/badge/GitHub%20Pages-Ready-brightgreen.svg)

An interactive biochemical and kinetic simulator of the **Calvin-Benson-Bassham ($\text{C}_3$ Reductive Pentose Phosphate) Cycle** across photoautotrophic plants, cyanobacteria, purple nonsulfur bacteria, and chemolithoautotrophic prokaryotes.

---

## ✨ Key Features

- **Full 13-Reaction Biochemical Network**:
  - **Phase 1 (Carbon Fixation)**: RuBisCO carboxylation vs. oxygenation ($\text{2-PG}$ photorespiratory branch).
  - **Phase 2 (Reduction)**: Phosphoglycerate kinase ($\text{PGK}$) and Glyceraldehyde-3-phosphate dehydrogenase ($\text{GAPDH}$).
  - **Phase 3 (Pentose Phosphate Regeneration Shuffle)**: Complete sugar-phosphate interconversion map ($\text{FBP}$, $\text{F6P}$, $\text{E4P}$, $\text{SBP}$, $\text{S7P}$, $\text{R5P}$, $\text{Xu5P}$, $\text{Ru5P}$) catalyzed by Aldolase, $\text{FBPase}$, Transketolase, $\text{SBPase}$, $\text{RPI/RPE}$, and $\text{PRK}$.
- **Competitive RuBisCO Michaelis-Menten Kinetics**:
  $$v_c = \frac{k_{\text{cat},c} \cdot [\text{CO}_2]}{[\text{CO}_2] + K_c\left(1 + \frac{[\text{O}_2]}{K_o}\right)}, \qquad v_o = \frac{k_{\text{cat},o} \cdot [\text{O}_2]}{[\text{O}_2] + K_o\left(1 + \frac{[\text{CO}_2]}{K_c}\right)}$$
- **Comparative Autotrophic Presets**:
  1. *Spinacia oleracea* ($\text{C}_3$ Chloroplast — Form IB $\text{L}_8\text{S}_8$ RuBisCO)
  2. *Synechococcus elongatus* (Cyanobacterium — Form IB inside a $\beta$-Carboxysome $\text{CCM}$)
  3. *Rhodospirillum rubrum* (Purple Nonsulfur Bacterium — Ancestral Dimeric Form II $\text{L}_2$ RuBisCO)
  4. *Acidithiobacillus ferrooxidans* (Chemolithoautotroph — Form IA inside an $\alpha$-Carboxysome)
- **Interactive Biochemical Inspector**: Click any intermediate or enzyme badge to inspect its EC number, $\Delta G'^\circ$, reaction stoichiometry, cofactors ($\text{Mg}^{2+}$, $\text{TPP}$), and Ferredoxin-Thioredoxin allosteric regulation.
- **CSV Telemetry Export**: Export kinetic parameters and cumulative $\text{ATP}/\text{NADPH}/\text{CO}_2$ balances directly to CSV.

---

## 🚀 Quick Start & GitHub Pages Deployment

This project requires **zero build steps** and runs natively in any modern browser.

### Run Locally
Clone the repository and open `index.html` in your browser:
```bash
git clone [https://github.com/YOUR-USERNAME/calvin-benson-simulator.git](https://github.com/YOUR-USERNAME/calvin-benson-simulator.git)
cd calvin-benson-simulator
open index.html
