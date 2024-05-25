# NeuroMechFly 2.0 Navigation Algorithm

## Abstract

This project develops a novel algorithm using NeuroMechFly 2.0 aimed at enabling the fly to navigate through various obstacle environments relying on mechanosensation. The algorithm focuses on scenarios where visual, olfactory, or other sensory capabilities are limited or non-functional, such as dark or tightly enclosed spaces. It includes a finely-tuned decision-making mechanism that facilitates turning and reversing based on mechanosensory feedback, thus enabling the fly to navigate complex environments effectively. The approaches are based on the Hybrid Turning Controller and basic reversing algorithms discussed in class.[^1]

## Introduction

_Drosophila melanogaster_, or the common fruit fly, utilizes complex structures within its legs, such as campaniform sensilla, to detect contact forces. Mechanosensory bristles, which are hair-like structures densely covering the legs, wings, and antennae, are pivotal in sensing mechanical forces. These forces trigger responses in sensory neurons that convey detailed information about location, direction, and intensity of stimuli to the brain, aiding in movement coordination.

The Neuromechfly algorithm emulates this by enabling each segment of the fly's lower leg—tibia and five tarsus segments—to detect contact forces separately. This design mimics the actual anatomical capabilities of the fruit fly, allowing for precise detection of force direction and magnitude in three dimensions. The project's algorithm aims to replicate complex natural behaviors such as exploring escape routes in the dark by feeling around with its legs, adjusting body posture to climb or fly over obstacles, and executing strategic reversals to make space for turning maneuvers.

## Project Structure

The repository is structured around five main Jupyter notebooks, each addressing different aspects of the simulation setup, development, and execution:

1. **1_Environment.ipynb**
   - This notebook focuses on the creation of the environment with obstacles, including both pillars and walls, setting the stage for the simulation scenarios.

2. **2_Contact_Forces.ipynb**
   - Building on the environment created in the first notebook, this file is dedicated to detecting forces exerted on the fly's legs. It guides through selecting which legs and leg segments to monitor for obstacle interaction and setting force thresholds based on the detected contact forces.

3. **3_Controller.ipynb**
   - Details the implementation of the control logic that manages the fly’s navigation based on sensor input and environmental interactions. This includes the logic for turning, moving backward and adjusting movements dynamically.

4. **4_Backward.ipynb**
   - This notebook explains the methodology behind the backward movement implementation, detailing how reversing maneuvers are integrated into the fly's behavior to handle obstacles.

5. **5_Complete_Machine.ipynb**
   - Contains the final simulation setup where all components from the previous notebooks are integrated. This notebook runs the full simulation demonstrating the fly’s navigation through the environment using the developed algorithm.
