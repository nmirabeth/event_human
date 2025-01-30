# Human-centered applications of event data 

This is the official repository of "Event-based solutions for human-centered applications: A comprehensive review" submitted to Frontiers in Signal Processing journal.

Event cameras, or dynamic vision sensors, capture changes in light intensity asynchronously, providing high temporal resolution and energy efficiency. These features make them ideal for human-centered applications, such as analyzing facial expressions and body motion dynamics. However, research in this area is fragmented. This repository unifies advancements in body and face-related tasks, offering a comprehensive review of databases, event data representation, and processing models. It serves as a foundational resource for researchers, guiding future work in human-centered event camera applications.

# Datasets

## Real event-based datasets for human-centered applications
### Body Datasets

| Year | Authors | Name | #Videos | #People | Modalities | Application | #Classes |
|------|---------|------|------------|----------|------------|-------------|-----------|
| 2019 | [Miao et al.](https://example.com) | Action Dataset TUM | 291 | 15 | EV | Action Recognition | 10
| 2019 | Goyal et al. [Link](https://example.com) | DHP19 | 2244 | 17 | EV | Pose Estimation | -
| 2019 | Wang et al. [Link](https://example.com) | DVS128-Gait-Day | 4000 | 20 | EV | Gait Recognition | -
| 2019 | Wang et al. [Link](https://example.com) | DVS128-Gait-Night | 4000 | 20 | EV | Gait Recognition | -
| 2021 | Liu et al. [Link](https://example.com) | DailyAction-DVS | 1440 | 15 | EV | Action Recognition | 12
| 2022 | Eddine and Dugelay [Link](https://example.com) | Gait3 | 168 | 56 | RGB-EV-TH | Gait Recognition | -
| 2023 | Gao et al. [Link](https://example.com) | THU-E-ACT-50 | 10500 | 105 | EV | Action Recognition | 50
| 2023 | Gao et al. [Link](https://example.com) | THU-E-ACT-50-CHL | 2330 | 18 | EV | Action Recognition | 50
| 2025 | Wang et al. [Link](https://example.com) | DailyDVS-200 | 22000 | 46 | RGB-EV | Action Recognition | 200
| 2024 | Gao et al. [Link](https://example.com) | THU-MV-E-ACT-50 | 31500 | 105 | EV | Action Recognition | 50

### Face Datasets

| Year | Authors | Name | #Videos | #People | Modalities | Application |
|------|---------|------|------------|----------|------------|-------------|
| 2016 | Barua et al. [Link](https://example.com) | - | - | 40 | EV | Face Detection 
| 2019 | Li et al. [Link](https://example.com) | - | 34000 | 34 | EV-audio | Lip Reading 
| 2020 | Angelopoulos et al. [Link](https://example.com) | - | 24 | 24 | EV | Eye gaze tracking
| 2020 | Chen et al. [Link](https://example.com) | EDDD | 260 | 26 | EV | Drowsiness 
| 2020 | Lenz et al. [Link](https://example.com) | - | 48 | 10 | EV | Face Detection 
| 2020 | Chen et al. [Link](https://example.com) | NeuroBiometric | 180 | 45 | EV | Authentication 
| 2022 | Banerjee et al. [Link](https://example.com) | - | 3360 | 6 | RGB-EV | Eye gaze tracking
| 2022 | Beccattini et al. [Link](https://example.com) | - | 455 | 25 | RGB-EV | MER 
| 2022 | Tan et al. [Link](https://example.com) | DVS-Lip | 19871 | 40 | EV | Lip Reading 
| 2022 | Moreira et al. [Link](https://example.com) | NVSFD | 436 | 40 | EV | Identity Recognition 
| 2023 | Bissarinova et al. [Link](https://example.com) | FES | ∼4000 | 73 | EV | Face Detection 
| 2023 | Berlincioni et al. [Link](https://example.com) | NEFER | 29 | 105 | RGB-EV | MER 
| 2023 | Kanamaru et al. [Link](https://example.com) | - | 1500 | 20 | EV | Lip Reading 
| 2024 | Adra et al. [Link](https://example.com) | VETEX | 2506 | 30 | RGB-EV-TH | MER


## Synthetic datasets for human-centered applications
### Body Datasets

| Year | Authors | Name | #Videos | #People | Application | #Classes |
|------|---------|------|---------|---------|-------------|----------|
| 2019 | Wang et al. [Link](https://example.com) | EV-CASIA-B | 8184 | 124 | Gait Recognition | -
| 2020 | Bi et al. [Link](https://example.com) | HMDB51-DVS | 6766 | - | Action Recognition | 51
| 2020 | Bi et al. [Link](https://example.com) | UCF101-DVS | 13320 | - | Action Recognition | 101
| 2022 | Plizzari et al. [Link](https://example.com) | N-EPIC-Kitchens | 64 | - | Action Recognition | 8
| 2023 | Zou et al. [Link](https://example.com) | SynEventHPD | 9197 | 47 | Pose Estimation | -
| 2023 | Goyal et al. [Link](https://example.com) | eH36m | 748 | 7 | Pose Estimation | -


### Face Datasets

| Year | Authors | Name | #Videos | #People | Application |
|------|---------|------|------------|----------|---------|
| 2022 | Moreira et al. [Link](https://example.com) | SynFED | 6536 | 30 | Identity Recognition 
| 2023 | Barchid et al. [Link](https://example.com) | ADFES | 198 | 22 | Face Expression Recognition
| 2023 | Barchid et al. [Link](https://example.com) | Oulu-CASIA | 480 | 80 | Face Expression Recognition
| 2023 | Barchid et al. [Link](https://example.com), Verschae and Bugueno-Cordova [Link](https://example.com) | e-CK+ | 327 | 93 | Face Expression Recognition
| 2023 | Barchid et al. [Link](https://example.com), Verschae and Bugueno-Cordova [Link](https://example.com) |e-MMI | 2900+ | 75 | Face Expression Recognition
| 2023 | Ryan et al. [Link](https://example.com) | - | - | 5 | Multitask Facial Analysis
| 2024 | Tan et al. [Link](https://example.com) | DVS-LRW100 | 107664 | - | Lip Reading

# Event Data Representations

| Name | Details | 
|------|---------|
| Event Count | Event data is aggregated by counting the number of events that occur at each pixel within a fixed time interval. This approach provides a straightforward summary of activity, often used as a baseline representation.
| Event Histogram | Similar to the event count, but instead of a single time interval, events are grouped and counted in temporal bins, creating a distribution of event activity that captures variations with more levels of detail.
| Time Surface / Surface of Active Events | Represents data as a continuous map where each pixel value corresponds to the most recent timestamp of an event at that location. This highlights recent activity and is often used to track motion or identify edges.
| Memory Surface | Event data are represented as a temporal map where each pixel’s value indicates the time elapsed since the last event occurred at that location within a fixed time window. This approach encodes temporal information by retaining a ”memory” of inactivity, making it useful for identifying patterns, and tracking regions with recent or ongoing motion. 
| Voxel Grid | Event data is sliced temporally into small time intervals, creating a sequence of event slices. These slices are then stacked into a 3D grid, where each voxel represents the activity in a spatial region during a specific time window. This allows for preserving both spatial and temporal resolution. 
| Spike Tensor | Represents data as binary tensors indicating the occurrence of spikes in specific spatiotemporal locations. The tensor is separated into two channels for positive and negative polarities.
| Graph | Represents data as a graph, where events are treated as nodes in a graph with polarity as the node feature. Then, edges are created between nodes to represent spatiotemporal relationships, often used for tasks like pattern recognition.
| E2VID Frame | Represents data as reconstructed frames by using neural networks to convert the sparse event stream into intensity frames. This allows event data to be used with traditional frame-based computer vision methods.
| Temporal Binary Representation | Events are first stacked together into intermediate binary representations where each pixel can be considered as a binary string. These frames are then grouped into a single frame by applying binary to decimal conversion. Most popular in face analysis applications.

# Model Architecture

### Papers presented in this survey, classified by the type of AI architecture used for their models

| SNN | Graph NN | CNN | Transformers | Not AI-based |
|-----|----------|-----|--------------|--------------|


# Applications

## Applications of event cameras for human data along with an exhaustive selection of relevant works for each category. The applications are categorized into two main areas: face and body.

### Body

| Human Tracking | Gait Recognition | Action Recognition | Pose Estimation |
|----------------|------------------|--------------------|-----------------|

### Face

| Face Detection | Identity Recognition | Lip Reading | Eye Blinking & Gaze | Microexpression & Emotion Recognition |
|----------------|----------------------|-------------|---------------------|---------------------------------------|

# Citing

-- Coming soon --

# Acknowledgement

This research is a part of the HEIMDALL project, funded by the BPI as part of the AAP I-Demo.
Additionally, the work was supported by the European Union’s Horizon Europe research and innovation program under Grant Agreement No 101094831 for the Converge-Telecommunications and Computer Vision Convergence Tools for Research Infrastructures project.

