# MH2000 Experiment Simulator

Interactive simulations of five thermodynamic measurement techniques from **MH2000 Experimental Methods, Lecture 1 – Thermodynamic Measurements** (KTH Royal Institute of Technology).

**▶ Open the simulator:** https://sudhanshukuthe.github.io/mh2000-simulator/

It runs in any web browser, on a laptop or a phone. No login, no installation.

---

## The experiments

| # | Simulation | Direct link | What you can do |
|---|---|---|---|
| 01 | **Pseudoisopiestic method** (Au–Cd sealed tube, two-zone furnace) | [#isopiestic](https://sudhanshukuthe.github.io/mh2000-simulator/#isopiestic) | Set the reservoir and sample temperatures, wait for constant mass, and record points to build the a<sub>Cd</sub>–x<sub>Cd</sub> curve. |
| 02 | **Transpiration method** (vapour pressure of liquid Cu) | [#transpiration](https://sudhanshukuthe.github.io/mh2000-simulator/#transpiration) | Run experiments at different carrier-gas flow rates and find the plateau between back-diffusion (low flow) and unsaturated gas (high flow). Compare Ar and He. |
| 03 | **C–CO–CO₂ equilibria** (controlled oxygen potential over graphite) | [#boudouard](https://sudhanshukuthe.github.io/mh2000-simulator/#boudouard) | Change temperature and inlet gas, with or without graphite, and read the outlet %CO, p<sub>CO₂</sub> and p<sub>O₂</sub>. |
| 04 | **H₂–H₂O equilibrium** (water bubbler, controlled p<sub>O₂</sub>) | [#hydrogen](https://sudhanshukuthe.github.io/mh2000-simulator/#hydrogen) | Set the dew point and furnace temperature and see whether Fe, Ni or Cr oxidises or stays metallic. |
| 05 | **Liquid–liquid equilibria** (impeller mixing, induced emulsification) | [#emulsion](https://sudhanshukuthe.github.io/mh2000-simulator/#emulsion) | Stir slag and liquid Si at different speeds and follow the interfacial area and the Ca transfer over time. |

Each simulation has the animated apparatus, controls, live readouts and a chart of your results. Double-click the apparatus to show it full screen when projecting.

## Suggested student exercises

1. **Pseudoisopiestic:** Record one point before equilibrium and one after. How far off is the early point, and why does the real Au–Mn study need 6–8 weeks?
2. **Transpiration:** Measure at 5, 20, 80 and 300 mL/min. Which flow rates give the true vapour pressure? What changes with He as the carrier gas?
3. **C–CO–CO₂:** Heat from 900 K to 1873 K with graphite present. Why can't an oxygen probe be used at 1873 K?
4. **H₂–H₂O:** For Fe at 1273 K, find the dew point at which FeO starts to form. Why does Cr oxidise even in very dry hydrogen?
5. **Slag–metal:** Compare 0, 50 and 100 rpm. Why does the interfacial area fall while mixing continues?

## Scientific basis

The calculations use the same thermodynamic data as the lecture slides:

- C(gr) + CO₂(g) = 2CO(g), ΔG° = 170 700 − 174.5T J
- 2CO(g) + O₂(g) = 2CO₂(g), ΔG° = −564 800 + 173.62T J
- H₂(g) + ½O₂(g) = H₂O(g), ΔG° = −246 450 + 54.8T J
- Cd and Cu vapour pressures from Clausius–Clapeyron fits; metal/oxide equilibria (Fe/FeO, Ni/NiO, Cr/Cr₂O₃) from standard compilations

**Simplified models.** These two parts are qualitative:

- The Au–Cd activity uses a regular-solution model (Ω = −40 kJ/mol).
- The emulsification kinetics reproduce the trends reported by White & Sichen (2014), not their absolute values.

Use them to understand the behaviour, not as reference data.

## References

- J. F. White, *Thermodynamic Measurements*, MH2000 lecture material, KTH.
- R. A. Rapp (ed.), *Physicochemical Measurements in Metals Research*, Part 1, Interscience, 1970.
- O. Kubaschewski, C. B. Alcock, P. J. Spencer, *Materials Thermochemistry*, 6th ed., Pergamon, 1993.
- J. White, D. Sichen, "Mass Transfer in Slag Refining of Silicon with Mechanical Stirring: Transient Interfacial Phenomena", *Metall. Mater. Trans. B*, 45B (2014) 96–105.
- J. P. Bartha, W. A. Alexander, *Can. J. Chem.* 43 (1965).

## Technical notes

- Everything is in one self-contained file, `index.html` (plain HTML, CSS and JavaScript, no build step). It also works offline if downloaded and opened locally.
- It is hosted with GitHub Pages from the `main` branch. To update the simulator, replace `index.html` and commit; the site refreshes within a minute or two.

## Author

Dr. Sudhanshu Kuthe, KTH Royal Institute of Technology. Released under the licence in [LICENSE](LICENSE).
