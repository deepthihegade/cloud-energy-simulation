# Energy Efficient Cloud Data Center Simulation

Cloud Computing Mini Project | REVA University | 2025-26

## What this does
Simulates a cloud data center using CloudSim Plus and compares 3 metaheuristic VM allocation algorithms for energy efficiency.

## Algorithms compared
- **ACO** (Ant Colony Optimization) - pheromone-guided VM placement
- **GA** (Genetic Algorithm) - fitness-based host selection  
- **PSO** (Particle Swarm Optimization) - weighted score-based placement

## Results
| Policy | LOW (kWh) | MEDIUM (kWh) | HIGH (kWh) | Total |
|--------|-----------|--------------|------------|-------|
| ACO ✓  | 0.00611   | 0.08700      | 0.76159    | 0.854 |
| GA     | 0.00638   | 0.09078      | 0.79470    | 0.891 |
| PSO    | 0.00664   | 0.09456      | 0.82782    | 0.929 |

**ACO is most energy efficient** by consolidating VMs onto fewer hosts.

## How to run
```bash
javac --release 17 -cp ".:jars/*" src/EnergySimulation.java -d .
java -cp ".:jars/*" EnergySimulation 2>/dev/null
```

## Tech stack
- Java 11+
- CloudSim Plus 8.0.0
EOF
git add README.md
git commit -m "add README"
git push
