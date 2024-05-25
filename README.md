# NeuroMechFly 2.0 Navigation Algorithm

## Abstract

This project develops a novel algorithm using NeuroMechFly 2.0 aimed at enabling the fly to navigate through various obstacle environments relying on mechanosensation. The algorithm focuses on scenarios where visual, olfactory, or other sensory capabilities are limited or non-functional, such as dark or tightly enclosed spaces. It includes a finely-tuned decision-making mechanism that facilitates turning and reversing based on mechanosensory feedback, thus enabling the fly to navigate complex environments effectively. The approaches are based on the Hybrid Turning Controller and basic reversing algorithms discussed in class.[^1]

## Introduction

_Drosophila melanogaster_, or the common fruit fly, utilizes complex structures within its legs, such as campaniform sensilla, to detect contact forces. Mechanosensory bristles, which are hair-like structures densely covering the legs, wings, and antennae, are pivotal in sensing mechanical forces. These forces trigger responses in sensory neurons that convey detailed information about location, direction, and intensity of stimuli to the brain, aiding in movement coordination.

The Neuromechfly algorithm emulates this by enabling each segment of the fly's lower leg—tibia and five tarsus segments—to detect contact forces separately. This design mimics the actual anatomical capabilities of the fruit fly, allowing for precise detection of force direction and magnitude in three dimensions. The project's algorithm aims to replicate complex natural behaviors such as exploring escape routes in the dark by feeling around with its legs, adjusting body posture to climb or fly over obstacles, and executing strategic reversals to make space for turning maneuvers.
