# Simulation Workshop 1 - Solution

This repository contains our solution for Simulation Workshop 1, implementing discrete-event simulation (DES) and process-based simulation models of a surgical unit. As Q group, we have analyzed the patient flow through preparation, surgery, and recovery phases, incorporating resource constraints and time-varying elements like staff shifts. This submission is ready for review by peers, other students, and professors.

## Team/Authors
Haben Eyasu
Ke Qiu
Ridwan Abdi

## Solution Overview

We implemented a comprehensive simulation model of the surgical unit system, focusing on both event-based and process-based approaches. Our solution addresses all required scenarios and provides detailed analysis of system performance under various conditions.

### Approach Taken
- **Primary Model**: Process-based simulation using [specify software/tool, e.g., SimPy/Python]
- **Secondary Analysis**: Event-based conceptual model for validation
- **Key Focus**: Time-varying capacities, blocking behavior, and statistical analysis

## Repository Contents

### Solution Documents
- `assignment-1-solution.pdf` - Our comprehensive solution combining event-based and process-based models, including specifications, implementation, lifecycle, resources, and experimental results

### Supporting Diagrams (Embedded in PDFs)
The following diagrams are embedded within the PDF documents and also available separately:
- `images/event-flow-diagram.png` - Event flow diagram for the surgical unit
- `images/example-parapmeter-set.png` - Example parameter configurations
- `images/life-cycle-sketch.png` - Patient lifecycle overview
- `images/life-cycle-steps-detailed.png` - Detailed process steps
- `images/modelling-paradigm.png` - Process-based modeling illustration
- `images/suggested-statistical-settings.png` - Statistical analysis guidelines

## Theoretical Analysis and Model Design

### System Components
- **Entities**: Patients and staffs with shift scheduling
- **Resources**: PrepPool (time-varying capacity), Theatre (single unit), RecoveryPool (time-varying)
- **Time Elements**: Day/night shifts, handover effects, variable arrival rates

### Key Features Analyzed
- Blocking behavior when recovery beds unavailable
- Time-varying resource capacities and their impact
- Statistical analysis methodology for multiple replications
- Performance metrics identification and calculation

## Conceptual Model Development

### Event-Based Approach
- Identified discrete events and state transitions
- Modeled doctor availability constraints
- Developed event flow diagrams and state variables

### Process-Based Approach
- Designed patient lifecycle with resource requests/releases
- Incorporated time-varying capacities and service rates
- Analyzed blocking behavior and queue management

## Theoretical Experimental Design

### Scenario Analysis Framework
1. **Baseline**: Fixed capacities - establishes reference performance
2. **Time-Varying Arrivals**: Day/night patterns - tests arrival variability effects
3. **Shift Capacities**: Staff reductions - evaluates capacity constraint impacts
4. **Recovery Sensitivity**: Bed capacity variations - analyzes blocking probability sensitivity
5. **Handover Effects**: Shift changes - examines transition period inefficiencies

### Expected Key Metrics
- **Average Throughput Time**: Total time from arrival to departure
- **Blocking Probability**: Fraction of time/frequency theatre is blocked
- **Theatre Utilization**: Effective use during available periods
- **Peak Queue Lengths**: Maximum waiting patients at each stage

### Theoretical Findings and Hypotheses
- Time-varying arrivals will increase peak period congestion
- Reduced nighttime capacities will create bottlenecks
- Recovery bed limitations will cause theatre blocking
- Shift handovers may introduce service time variability

## Model Validation Considerations
- Cross-validation between event-based and process-based approaches
- Sensitivity analysis on key parameters
- Statistical rigor with multiple replications
- Warm-up period analysis for steady-state assessment

## Implementation Planning
- Software selection criteria (SimPy, Arena, AnyLogic, or custom)
- Data collection and statistical analysis framework
- Validation and verification procedures
- Result presentation and interpretation guidelines

## Theoretical Challenges Identified
- Modeling time-varying capacities accurately
- Capturing blocking behavior correctly
- Ensuring statistical validity with limited replications
- Balancing model complexity with computational efficiency

## Learning Outcomes
- Deepened understanding of discrete-event simulation principles
- Gained experience in healthcare system modeling
- Developed skills in performance analysis and bottleneck identification
- Learned to design experiments with statistical rigor

## Model Documentation
Implementation details and theoretical models are fully documented in the PDF file, providing complete specifications for future coding implementation.

## References
- Stewart Robinson (2004). Simulation – The practice of model development and use. Wiley.
- SoftwareSim. (2022). A gentle introduction to discrete event simulation.
- [Any additional references used]

## How to Review This Solution

1. Start with the PDF document for our model specifications
2. Review the diagrams for visual understanding
3. Examine our experimental results and analysis
5. Suggest improvements or alternative approaches

Thank you for reviewing our work! We look forward to your feedback and learning from the review process.
