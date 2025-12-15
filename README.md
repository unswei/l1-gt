# L1-GT/500 (L1 gyro trolley)

L1-GT is an open, wheeled-biped research platform. It is developed within the Embodied Intelligence & Collective Robotics studio (EICR) at UNSW.

The platform explores dynamically stable mobility using a two-wheeled base combined with articulated leg structures and a modular upper body. It is inspired by earlier work on wheeled inverted-pendulum robots, including Fraunhofer IML’s evoBOT, and by more recent open platforms such as Upkie.

The aim is not to optimise for a single task, but to provide a practical, buildable system for studying embodied control, learning, and robustness under real-world physical constraints.

---

## project status

- **hardware:** initial design near complete (v0.x)
- **electronics:** in development
- **software and control:** in development

This repository currently focuses on the mechanical design. Electronics, software, and control will be added as the project matures.

---

## motivation

Many results in robot learning and control rely heavily on simulation fidelity or simplified dynamics. L1-GT is intended as a platform where modelling error, contact, balance, and sensing noise are unavoidable and measurable.

The design emphasises:
- physical embodiment as part of the control problem
- data-efficient learning in contact-rich settings
- robustness rather than peak performance

L1-GT is developed as research infrastructure. It is meant to be modified, rebuilt, and extended.

---

## research directions enabled

The platform supports research in areas including:

- whole-body balancing and locomotion under uncertainty  
- hybrid control and learning approaches combining physical models and data  
- morphology and mechanism design as control resources  
- benchmarking classical control, optimisation-based methods, and learning-based approaches on identical hardware  
- embodied intelligence questions where shape, actuation, and sensing materially affect what can be learned

The intent is to support both algorithmic work and studies that explicitly link mechanical design choices to control and learning outcomes.

---

## repository structure

The repository is organised by major subsystems. Each component has its own documentation, CAD, and bill of materials.

```text
README.md

hardware/
├── wheels/
│   ├── README.md
│   ├── cad/
│   ├── drawings/
│   ├── bom/
│   └── assembly/
├── legs/
│   ├── README.md
│   ├── cad/
│   ├── drawings/
│   ├── bom/
│   └── assembly/
├── arms/
│   ├── README.md
│   ├── cad/
│   ├── drawings/
│   ├── bom/
│   └── assembly/
├── bridge/
│   ├── README.md
│   ├── cad/
│   ├── drawings/
│   ├── bom/
│   └── assembly/
└── shell/
    ├── README.md
    ├── cad/
    ├── drawings/
    ├── bom/
    └── assembly/

docs/
├── README.md
├── system-overview.md
├── interfaces.md
├── build-philosophy.md
└── faq.md
```


Each hardware component directory typically contains:
- a short README describing the component
- CAD files and drawings
- a BOM with supplier references
- assembly and integration notes
- known issues and limitations

---

## documentation

The main entry point is this README.  
Detailed documentation lives alongside the design files in each subdirectory.

---

## licensing

Different artefacts in this repository use different licences:

- **hardware design files (CAD, drawings, mechanical design):**  
  CERN Open Hardware Licence v2.0 – Weakly Reciprocal (CERN-OHL-W)

- **software:**  
  Apache Licence 2.0

- **documentation and original images:**  
  Creative Commons Attribution 4.0 (CC BY 4.0)

See the `LICENSES/` directory for full licence texts.

---

## citation

If you use L1-GT in academic work, please cite it.  
A `CITATION.cff` file is provided to support standard citation workflows.

---

## related work and inspiration

- Fraunhofer IML evoBOT  
- Upkie open wheeled-biped robot  
- Independent wheeled-biped projects such as *Impulse* by Aaed Musa

These projects influenced the design space explored here, but L1-GT makes its own mechanical and architectural trade-offs.

---

## contributions

Contributions are welcome, particularly:
- build notes and corrections
- BOM substitutions
- mechanical improvements
- calibration data and failure reports

Please see `CONTRIBUTING.md` for details.

---

## acknowledgements

L1-GT is developed and built as a research platform for embodied Intelligence & collective robotics at UNSW.

---

