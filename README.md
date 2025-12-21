# MadGraph Event Generation Cards  
*(CMS-inspired configurations for realistic LHC simulations)*

## Overview
This repository contains a collection of **MadGraph5_aMC@NLO** event generation setups for **proton–proton collisions at √s = 13–13.6 TeV**, designed to closely follow **CMS simulation conventions**.

Each process includes a full set of **carefully edited MadGraph cards**, inspired by CMS-recommended settings for:
- Physics process definitions  
- Parton-level generation  
- Spin correlations  
- Parton showering and hadronization  
- Realistic tune choices (e.g. **TuneCP5** with **PYTHIA8**)

The purpose of this repository is to provide **reproducible, well-documented, and analysis-ready event generation configurations** suitable for phenomenological studies and experimental high-energy physics analyses.

---

## Repository Structure

- **`Cards/`**  
  Contains all MadGraph process directories.
- Each directory corresponds to **one specific physics process** generated using MadGraph.
# MadGraph Event Generation Cards  
*(CMS-inspired configurations for realistic LHC simulations)*

## Overview
This repository contains a collection of **MadGraph5_aMC@NLO** event generation setups for **proton–proton collisions at √s = 13–13.6 TeV**, designed to closely follow **CMS simulation conventions**.

Each process includes a full set of **carefully edited MadGraph cards**, inspired by CMS-recommended settings for:
- Physics process definitions  
- Parton-level generation  
- Spin correlations  
- Parton showering and hadronization  
- Realistic tune choices (e.g. **TuneCP5** with **PYTHIA8**)

The purpose of this repository is to provide **reproducible, well-documented, and analysis-ready event generation configurations** suitable for phenomenological studies and experimental high-energy physics analyses.

---

## Repository Structure
- **`Cards/`**  
  Contains all MadGraph process directories.
- Each directory corresponds to **one specific physics process** generated using MadGraph.

---

## Process Directory Structure
Each process folder (e.g. `PP_thb_NLO_TuneCP5_13-6_TeV_pythia8`) contains the following standard MadGraph card files:

| File name | Description |
|----------|-------------|
| `proc_card.dat` | Definition of the physics process and generation commands |
| `param_card.dat` | Model parameters (masses, widths, couplings) |
| `run_card.dat` | Run-level configuration (beam energy, cuts, scales, PDFs, event settings) |
| `madspin_card.dat` | Spin correlations and particle decays using **MadSpin** |
| `shower_card.dat` | Parton shower and hadronization settings (PYTHIA8, CMS-tuned) |

---

## CMS-Inspired Configuration
The cards in this repository are **not default MadGraph templates**. They have been **explicitly edited** to reflect realistic CMS simulation practices, including:

- CMS-preferred **PYTHIA8 tunes** (e.g. TuneCP5)
- Realistic beam energies (13–13.6 TeV)
- Appropriate scale choices and matching schemes
- Proper treatment of decays using **MadSpin**
- Showering configurations compatible with CMS workflows

These settings are intended to produce **analysis-quality Monte Carlo samples**, suitable for further processing (e.g. detector simulation, slim trees, and physics analysis).

---

## Physics Scope
The processes included in this repository are relevant to **LHC Run 2 and Run 3 physics analyses**, particularly in the context of:
- Higgs physics
- Single-top and top-associated production
- Background modeling for multijet and heavy-flavor final states

The configurations are suitable for both **phenomenological studies** and **experimental analysis preparation**.

---

## Process Naming Convention
Process directories follow a descriptive naming scheme to ensure clarity and reproducibility:

`PP_<process>_<order>_<tune>_<energy>_pythia8`

Example:
- `PP_thb_NLO_TuneCP5_13-6_TeV_pythia8`

This convention encodes:
- Initial state (pp collisions)
- Physics process
- Perturbative order (LO/NLO)
- Parton shower tune
- Center-of-mass energy

---

## Software and Configuration
- Event generator: **MadGraph5_aMC@NLO**
- Parton shower: **PYTHIA8**
- Tune: **CMS TuneCP5**
- Collision energy: **√s = 13–13.6 TeV**
- Spin correlations: **MadSpin**

PDF sets, scale choices, and matching schemes are specified explicitly in the corresponding `run_card.dat`.

---

## How to Use
1. Install **MadGraph5_aMC@NLO** (tested with recent versions).
2. Copy the desired process directory from `Cards/`.
3. Launch MadGraph:
   ```bash
   ./bin/mg5_aMC

---

## Process Directory Structure
Each process folder (e.g. `PP_thb_NLO_TuneCP5_13-6_TeV_pythia8`) contains the following standard MadGraph card files:

| File name | Description |
|----------|-------------|
| `proc_card.dat` | Definition of the physics process and generation commands |
| `param_card.dat` | Model parameters (masses, widths, couplings) |
| `run_card.dat` | Run-level configuration (beam energy, cuts, scales, PDFs, event settings) |
| `madspin_card.dat` | Spin correlations and particle decays using **MadSpin** |
| `shower_card.dat` | Parton shower and hadronization settings (PYTHIA8, CMS-tuned) |

---

## CMS-Inspired Configuration
The cards in this repository are **not default MadGraph templates**. They have been **explicitly edited** to reflect realistic CMS simulation practices, including:

- CMS-preferred **PYTHIA8 tunes** (e.g. TuneCP5)
- Realistic beam energies (13–13.6 TeV)
- Appropriate scale choices and matching schemes
- Proper treatment of decays using **MadSpin**
- Showering configurations compatible with CMS workflows

These settings are intended to produce **analysis-quality Monte Carlo samples**, suitable for further processing (e.g. detector simulation, slim trees, and physics analysis).

## About Me
I am **Malhar**, an **M.Phil. student at the National Centre for Physics (NCP), Islamabad**, currently pursuing my M.Phil. in **Experimental High Energy Physics**.

My research training and interests are closely aligned with **CERN CMS–related analyses**, with hands-on experience in Monte Carlo event generation, CMS-inspired simulation workflows, and collider data analysis tools. I am a PhD candidate in experimental particle physics aiming to contribute to precision measurements and searches at the LHC and future collider experiments.

