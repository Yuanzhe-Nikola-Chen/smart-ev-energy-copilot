# Smart EV Energy Copilot: Optimization for Energy-Aware Systems

This project presents a control- and optimization-oriented study of EV charging in residential energy systems, focusing on cost-efficient and constraint-aware energy management.

The system models interactions between:
- Electric vehicles (EVs)
- Household electricity demand
- Solar PV generation
- Time-varying electricity prices

The goal is to understand how optimization methods can coordinate energy flows under real-world constraints.

---

## Method

The system is formulated as a linear programming (LP) problem using PuLP.

**Objective**: Minimize total electricity cost

min Σ [price_buy(t) * grid_import(t) - price_sell(t) * grid_export(t)]

**Decision Variables**:
- Charging power p(t)
- Grid import/export
- Battery state of charge SOC(t)

**Constraints**:
- Power balance between PV, grid, load, and EV
- SOC dynamics and limits
- Charging power limits
- Final SOC target

---

## Features

- Linear programming-based optimization (PuLP)
- Time-of-use electricity pricing
- PV generation and home load modeling
- EV charging scheduling
- Output visualization (power and SOC curves)

---

## Research Context

This project explores energy-aware optimization in cyber-physical systems.

It reflects broader research questions:
- How to coordinate energy systems under constraints
- How optimization interacts with real-time decision-making
- How to scale from single-device control to system-level coordination

---

## Installation

pip install -r requirements.txt

---

## Usage

Run simulation:

python src/energycopilot/simulate.py

---

## Future Work

- Multi-vehicle coordination
- Real-world data integration
- V2G (vehicle-to-grid) modeling
- Stochastic and uncertainty-aware optimization

---

## Notes

This is a research-oriented demonstration of optimization methods in energy systems, focusing on system-level understanding rather than production deployment.

---

## 🎯 Research Directions

This project is aligned with research topics including:

* Autonomous Driving
* Robotics & Embodied Intelligence
* Optimal Control & MPC
* Intelligent Transportation Systems
* Energy-aware AI systems

---

## 👤 Author

**Yuanzhe (Nikola) Chen**

PhD Applicant (Fall 2027, United States preferred) | Autonomous Driving & Robotics | Control, Planning & Energy Systems | M.Eng (EE) @ UNSW

Research interests:

* Autonomous Driving & Robotics
* Control Theory & Optimal Control
* EV Energy Systems & Optimization

---

## 📬 Contact

Feel free to reach out for collaboration or discussion:

🔗 LinkedIn: www.linkedin.com/in/yuanzhe-chen-6b2158351

---

## License

MIT License
