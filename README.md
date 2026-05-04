# Research Lab v5 — Advanced Interactive Simulation Environment

Research Lab v5 is a single-file browser simulation for experimenting with artificial life, multi-agent behaviour, adaptive ecosystems, neural decision-making, open-ended evolution, and interactive environmental design.

It keeps the original simulation features — agents, food, threats, tasks, obstacles, controls, stats, logs, and real-time rendering — while adding layered research-lab systems such as learning agents, quality-diversity archives, cellular fields, Red Queen coevolution, social learning, signal communication, micro-experiments, habitat engineering, and closed-loop intervention.

---

## What Makes v5 Different

Research Lab v5 is not just a random moving-dot simulation. It is designed like a small artificial-life sandbox where agents, threats, resources, fields, and tasks interact over time.

The simulation now includes:

- Adaptive agents with energy, health, memory, traits, learning, reproduction, and mutation.
- Dynamic threats that can become more dangerous when agents dominate.
- Food, tasks, obstacles, brush tools, local fields, and manual world editing.
- A research director that watches the world and injects curriculum pressure.
- Quality-diversity tracking so different behavioural niches can survive.
- Social learning, symbiosis, signal fields, and habitat improvement mechanics.
- Save/load, import/export, snapshots, theater mode, inspect mode, and live metrics.

---

## Core Features

### Multi-Agent Ecosystem

Agents move through a 2D environment while trying to survive, gather food, avoid threats, complete tasks, and reproduce.

Agents have:

- Health
- Energy
- Speed
- Vision
- Curiosity
- Sustainability awareness
- Generation number
- Lineage information
- Behavioural traits
- Memory
- Learning state
- Fitness score

### Threats

Threats move through the world and damage agents on contact. Their behaviour can be affected by the Red Queen coevolution system, causing them to become more aggressive when agents are performing too well.

### Food and Resources

Food restores agent health and energy. Resource levels are affected by the environment, agent behaviour, and fertility fields.

### Tasks

Tasks act as environmental goals. Agents can complete tasks for rewards, and the research director can create new tasks to push the ecosystem into new behaviours.

### Obstacles

Obstacles block and shape movement. They can be added manually with brush tools and used to create mazes, barriers, safe zones, or stress-test environments.

---

## Research-Inspired Systems

### 1. Open-Ended Research Director

The research director watches the simulation and tries to prevent boring outcomes such as total collapse, overpopulation, stagnation, or under-exploration.

It can introduce new pressure through:

- Extra tasks
- Resource shifts
- New danger zones
- Micro-experiments
- Habitat challenges
- Curriculum events

### 2. Red Queen Coevolution

When agents become too successful, threats can adapt. This creates an arms-race effect where survival is not permanently solved.

### 3. Quality-Diversity Archive

The simulation tracks multiple behavioural niches instead of only rewarding one “best” agent type. This helps maintain variety across generations.

Example niches may include:

- Explorers
- Survivors
- Fast agents
- Sustainable agents
- Task-focused agents
- Risk-takers
- Efficient feeders

### 4. Neural / Learned Behaviour

Agents use lightweight neural-style decision logic, memory, and data augmentation to adapt movement decisions based on what they encounter.

The system keeps the earlier learning features and improves them with broader augmentation and safer runtime behaviour.

### 5. Cellular Field Layer

The world contains local field-like layers that influence agent behaviour and ecosystem conditions.

Field examples include:

- Nutrient
- Danger
- Trail
- Fertility
- Signal
- Hormone / cooperation pressure

These fields create indirect interactions between agents and the environment.

### 6. Social Learning

Agents can learn from nearby stronger agents. This allows useful behaviour to spread without every agent needing to discover it alone.

### 7. Symbiotic Guilds

Agents can form local support relationships. These guild-like links help weaker or specialised agents survive in stressful conditions.

### 8. Epigenetic Plasticity

Agents can adjust some traits during their lifetime in response to stress, hunger, danger, or resource availability.

### 9. Habitat Engineering

Sustainability-focused agents can improve local fertility and help restore parts of the environment.

### 10. Ghost Probes and Micro-Experiments

The simulation can test possible future task locations and create micro-experiments in promising or underexplored areas.

---

## Interface Features

### Main Canvas

The canvas displays the ecosystem in real time.

Common visual elements:

| Colour / Object | Meaning |
|---|---|
| Agent dots | Living agents |
| Red entities | Threats |
| Green entities | Food |
| Yellow entities | Tasks |
| Grey blocks | Obstacles |
| Field overlays | Environmental pressure, fertility, danger, signals, or trails |

### Stats Panel

The stats panel tracks live world information such as:

- Agent count
- Threat count
- Food count
- Task count
- FPS
- Step time
- Generation progress
- Best score
- Species count
- Symbiosis links
- Stability
- Habitat projects
- Alarm state

### Event Log

The event log records important events such as:

- Simulation resets
- Agent learning
- Agent deaths
- Task creation
- Habitat projects
- Red Queen pressure
- Research director interventions
- Micro-experiments
- Save/load actions

The log is capped so it does not grow forever.

---

## Controls

The exact controls may vary slightly depending on the version layout, but v5 includes the following major control groups.

### Simulation Controls

- Start / pause simulation
- Reset simulation
- Create environmental task
- Run micro-experiment
- Seed habitat
- Save state
- Load state
- Export JSON
- Import JSON
- Take snapshot

### Agent Controls

- Agent speed
- Max speed
- Energy decay
- Agent population pressure
- Learning / adaptation pressure

### Environment Controls

- Food count
- Threat count
- Obstacle count
- Field visibility
- Day/night cycle
- Scenario selection

### Brush Tools

Brush tools allow manual editing of the world.

Typical brush actions include:

- Add food
- Add threats
- Add tasks
- Add obstacles
- Add fertility
- Add danger
- Erase objects
- Inspect agents or locations

---

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| Space | Pause / resume |
| X | Run a micro-experiment |
| H | Seed habitat |
| I | Toggle inspect mode, if enabled |
| T | Toggle theater / minimal HUD mode, if enabled |
| S | Save, if enabled by the build |
| L | Load, if enabled by the build |

---

## Scenarios

Research Lab v5 includes multiple starting configurations for different experiments.

Examples:

### Balanced Ecosystem

A general-purpose world with moderate food, threats, tasks, and obstacles.

### Collapse Recovery

A stressful world designed to test whether the system can recover from low resources or high danger.

### Frontier Curriculum

A curriculum-style environment where tasks and resources encourage exploration into new regions.

### Symbiosis Stress Test

A world designed to test whether guilds, social learning, cooperation signals, and habitat engineering can help agents survive.

---

## How to Use

1. Open the HTML file in a modern browser.
2. Let the simulation run for a few seconds.
3. Watch agents, threats, food, tasks, and fields interact.
4. Use the sliders to change the world.
5. Add tasks, food, obstacles, or danger using brush tools.
6. Try different scenarios.
7. Save or export interesting worlds.
8. Use inspect mode to study agents.
9. Use snapshots to capture the current simulation state.

No build step is required.

---

## Installation

Download the HTML file and open it directly:

```text
advanced_sim_research_lab_v5.html
```

Recommended browsers:

- Chrome
- Edge
- Firefox
- Brave

Because this is a browser-based simulation, performance depends on your device and browser.

---

## Running Locally

You can run it by double-clicking the HTML file.

For a local server, use one of these options:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

Or use any simple static server.

---

## File Structure

Research Lab v5 is designed as a single-file project.

```text
advanced_sim_research_lab_v5.html
```

The file contains:

- HTML layout
- CSS styling
- Canvas rendering
- Simulation logic
- Agent classes
- Environment systems
- UI controls
- Save/load tools
- Research-inspired mechanics

---

## Feature Preservation Checklist

v5 keeps the major features from the full project history.

| Feature | Included |
|---|---|
| Agents | Yes |
| Threats | Yes |
| Food | Yes |
| Tasks | Yes |
| Obstacles | Yes |
| Day/night cycle | Yes |
| Stats panel | Yes |
| Event log | Yes |
| Performance metrics | Yes |
| Agent learning | Yes |
| Memory and data augmentation | Yes |
| Energy decay | Yes |
| Evolution and reproduction | Yes |
| Quality-diversity archive | Yes |
| Cellular fields | Yes |
| Save/load | Yes |
| JSON import/export | Yes |
| Snapshot rendering | Yes |
| Brush tools | Yes |
| Inspect mode | Yes |
| Theater/minimal HUD | Yes |
| Research director | Yes |
| Red Queen pressure | Yes |
| Social learning | Yes |
| Signal communication | Yes |
| Ghost probes | Yes |
| Micro-experiments | Yes |
| Habitat engineering | Yes |
| Symbiotic guilds | Yes |
| Epigenetic plasticity | Yes |

---

## Suggested Experiments

Try these experiments to see how the system behaves.

### 1. High Threat Pressure

Increase threats and aggressiveness. Watch whether agents evolve toward avoidance, grouping, or collapse.

### 2. Low Food World

Reduce food and increase energy decay. Watch whether sustainability, cooperation, or habitat engineering becomes more important.

### 3. Maze World

Use obstacle brushes to create corridors. Observe whether agents learn useful movement paths.

### 4. Task-Rich Curriculum

Create many tasks in different regions. Watch whether agents explore more widely.

### 5. Symbiosis Challenge

Use the Symbiosis Stress Test scenario and observe whether social links improve stability.

### 6. Red Queen Race

Let agents dominate, then watch how threat pressure adapts in response.

---

## Design Goals

Research Lab v5 is built around these goals:

- Keep the project single-file and easy to run.
- Preserve all previous features.
- Make the simulation more interactive.
- Add research-inspired systems that create richer emergent behaviour.
- Avoid fake UI buttons that do nothing.
- Make the world easier to inspect, save, load, and experiment with.
- Support both casual play and experimental observation.

---

## Limitations

This is a browser simulation, not a full scientific simulator.

Current limitations:

- Results are approximate and designed for exploration.
- Agent learning is lightweight, not a full-scale reinforcement learning system.
- Large populations can reduce FPS.
- Behaviour can be chaotic and depends on random initial conditions.
- Browser/device performance affects simulation speed.

---

## Future Ideas

Possible next upgrades:

- Replay timeline and rewind system.
- Graph panel for population, food, threat, and task history.
- Agent family tree viewer.
- More complex genomes.
- Real pathfinding experiments.
- Predator-prey specialisation.
- Multi-layer terrain.
- Weather and seasonal cycles.
- Evolutionary tournament mode.
- Better visual analytics.
- Web worker performance mode.
- Optional WebGL renderer.

---

## Credits

Created as an experimental single-file artificial-life and multi-agent simulation project.

Research inspirations include:

- Artificial life
- Open-ended evolution
- Quality-diversity search
- Neuroevolution
- Multi-agent learning
- Cellular automata
- Neural cellular automata
- Emergent cooperation
- Curriculum generation
- Ecological simulation

---

## License

Use, modify, and extend this project freely unless you add your own license terms.
