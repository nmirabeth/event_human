# Human-centered applications of event data 

This is the official repository of "Event-based solutions for human-centered applications: A comprehensive review" submitted to Frontiers in Signal Processing journal.

Event cameras, or dynamic vision sensors, capture changes in light intensity asynchronously, providing high temporal resolution and energy efficiency. These features make them ideal for human-centered applications, such as analyzing facial expressions and body motion dynamics. However, research in this area is fragmented. This repository unifies advancements in body and face-related tasks, offering a comprehensive review of databases, event data representation, and processing models. It serves as a foundational resource for researchers, guiding future work in human-centered event camera applications.

# Datasets

## Real event-based datasets for human-centered applications
### Body Datasets

| Year | Authors | Name | #Videos | #People | Modalities | Application | #Classes |
|------|---------|------|------------|----------|------------|-------------|-----------|
| 2019 | [Miao et al.](#miao) | Action Dataset TUM | 291 | 15 | EV | Action Recognition | 10
| 2019 | [Goyal et al.](#miao) | DHP19 | 2244 | 17 | EV | Pose Estimation | -
| 2019 | [Wang et al.](#miao) | DVS128-Gait-Day | 4000 | 20 | EV | Gait Recognition | -
| 2019 | [Wang et al.](#miao) | DVS128-Gait-Night | 4000 | 20 | EV | Gait Recognition | -
| 2021 | [Liu et al.](#miao) | DailyAction-DVS | 1440 | 15 | EV | Action Recognition | 12
| 2022 | [Eddine and Dugelay](#miao) | Gait3 | 168 | 56 | RGB-EV-TH | Gait Recognition | -
| 2023 | [Gao et al.](#miao) | THU-E-ACT-50 | 10500 | 105 | EV | Action Recognition | 50
| 2023 | [Gao et al.](#miao)| THU-E-ACT-50-CHL | 2330 | 18 | EV | Action Recognition | 50
| 2025 | [Wang et al.](#miao) | DailyDVS-200 | 22000 | 46 | RGB-EV | Action Recognition | 200
| 2024 | [Gao et al.](#miao) | THU-MV-E-ACT-50 | 31500 | 105 | EV | Action Recognition | 50

### Face Datasets

| Year | Authors | Name | #Videos | #People | Modalities | Application |
|------|---------|------|------------|----------|------------|-------------|
| 2016 | [Barua et al.](#miao) | - | - | 40 | EV | Face Detection 
| 2019 | [Li et al.](#miao) | - | 34000 | 34 | EV-audio | Lip Reading 
| 2020 | [Angelopoulos et al.](#miao) | - | 24 | 24 | EV | Eye gaze tracking
| 2020 | [Chen et al.](#miao) | EDDD | 260 | 26 | EV | Drowsiness 
| 2020 | [Lenz et al.](#miao) | - | 48 | 10 | EV | Face Detection 
| 2020 | [Chen et al.](#miao) | NeuroBiometric | 180 | 45 | EV | Authentication 
| 2022 | [Banerjee et al.](#miao) | - | 3360 | 6 | RGB-EV | Eye gaze tracking
| 2022 | [Beccattini et al.](#miao) | - | 455 | 25 | RGB-EV | MER 
| 2022 | [Tan et al.](#miao) | DVS-Lip | 19871 | 40 | EV | Lip Reading 
| 2022 | [Moreira et al.](#miao) | NVSFD | 436 | 40 | EV | Identity Recognition 
| 2023 | [Bissarinova et al.](#miao) | FES | ∼4000 | 73 | EV | Face Detection 
| 2023 | [Berlincioni et al.](#miao) | NEFER | 29 | 105 | RGB-EV | MER 
| 2023 | [Kanamaru et al.](#miao) | - | 1500 | 20 | EV | Lip Reading 
| 2024 | [Adra et al.](#miao) | VETEX | 2506 | 30 | RGB-EV-TH | MER


## Synthetic datasets for human-centered applications
### Body Datasets

| Year | Authors | Name | #Videos | #People | Application | #Classes |
|------|---------|------|---------|---------|-------------|----------|
| 2019 | [Wang et al.](#miao)| EV-CASIA-B | 8184 | 124 | Gait Recognition | -
| 2020 | [Bi et al.](#miao) | HMDB51-DVS | 6766 | - | Action Recognition | 51
| 2020 | [Bi et al.](#miao) | UCF101-DVS | 13320 | - | Action Recognition | 101
| 2022 | [Plizzari et al.](#miao) | N-EPIC-Kitchens | 64 | - | Action Recognition | 8
| 2023 | [Zou et al.](#miao) | SynEventHPD | 9197 | 47 | Pose Estimation | -
| 2023 | [Goyal et al.](#miao) | eH36m | 748 | 7 | Pose Estimation | -


### Face Datasets

| Year | Authors | Name | #Videos | #People | Application |
|------|---------|------|------------|----------|---------|
| 2022 | [Moreira et al.](#miao)| SynFED | 6536 | 30 | Identity Recognition 
| 2023 | [Barchid et al.](#miao) | ADFES | 198 | 22 | Face Expression Recognition
| 2023 | [Barchid et al.](#miao) | Oulu-CASIA | 480 | 80 | Face Expression Recognition
| 2023 | [Barchid et al.](#miao) ; [Verschae and Bugueno-Cordova](#miao) | e-CK+ | 327 | 93 | Face Expression Recognition
| 2023 | [Barchid et al.](#miao) ; [Verschae and Bugueno-Cordova](#miao) |e-MMI | 2900+ | 75 | Face Expression Recognition
| 2023 | [Ryan et al.](#miao) | - | - | 5 | Multitask Facial Analysis
| 2024 | [Tan et al.](#miao) | DVS-LRW100 | 107664 | - | Lip Reading

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



| SNN                          | Graph NN                     | CNN                          | Transformers                 | Not AI-based                 |
|------------------------------|------------------------------|------------------------------|------------------------------|------------------------------|
| [Liu et al. (2021)](#liu2021) | [Wang et al. (2021)](#wang2021) | [Li et al. (2019)](#li2019)   |   [Xu et al. (2020)](#xu2020)                         | [Barua et al. (2016)](#barua2016) |
| [Barchid et al. (2023)](#barchid2023) | [Eisl et al. (2023)](#eisl2023) | [Wang et al. (2019)](#wang2019) |                              | [Savran et al. (2018)](#savran2018) |
|                              |                              | [Sokolova and Konushin (2019)](#sokolova2019) |                              | [Lenz et al. (2020)](#lenz2020) |
|                              |                              | [Ryan et al. (2021)](#ryan2021) |                              |                              |
|                              |                              | [Banerjee et al. (2022)](#banerjee2022) |                              |                              |
|                              |                              | [Becattini et al. (2022)](#becattini2022) |                              |                              |
|                              |                              | [Moreira et al. (2022)](#moreira2022) |                              |                              |



# Applications

### Applications of event cameras for human data along with an exhaustive selection of relevant works for each category. The applications are categorized into two main areas: face and body.

### Body

| Human Tracking | Gait Recognition | Action Recognition | Pose Estimation |
|----------------|------------------|--------------------|-----------------|

### Face

| Face Detection | Identity Recognition | Lip Reading | Eye Blinking & Gaze | Microexpression & Emotion Recognition |
|----------------|----------------------|-------------|---------------------|---------------------------------------|

# Citing

## Bibliography

- <a id="miao"></a> Miao, S., Chen, G., Ning, X., Zi, Y., Ren, K., Bing, Z., et al. (2019). Neuromorphic vision datasets for pedestrian detection, action recognition, and fall detection
- <a id="liu2021"></a>Liu et al. (2021). [Title of the paper](URL_to_paper).
- <a id="barchid2023"></a>Barchid et al. (2023). [Title of the paper](URL_to_paper).
- <a id="wang2021"></a>Wang et al. (2021). [Title of the paper](URL_to_paper).
- <a id="eisl2023"></a>Eisl et al. (2023). [Title of the paper](URL_to_paper).
- <a id="li2019"></a>Li et al. (2019). [Title of the paper](URL_to_paper).
- <a id="xu2020"></a>Xu et al. (2020). [Title of the paper](URL_to_paper).
- <a id="barua2016"></a>Barua et al. (2016). [Title of the paper](URL_to_paper).
- <a id="savran2018"></a>Savran et al. (2018). [Title of the paper](URL_to_paper).
- <a id="lenz2020"></a>Lenz et al. (2020). [Title of the paper](URL_to_paper).
- <a id="sokolova2019"></a>Sokolova and Konushin (2019). [Title of the paper](URL_to_paper).
- <a id="ryan2021"></a>Ryan et al. (2021). [Title of the paper](URL_to_paper).
- <a id="banerjee2022"></a>Banerjee et al. (2022). [Title of the paper](URL_to_paper).
- <a id="becattini2022"></a>Becattini et al. (2022). [Title of the paper](URL_to_paper).
- <a id="moreira2022"></a>Moreira et al. (2022). [Title of the paper](URL_to_paper).


# Acknowledgement

This research is a part of the HEIMDALL project, funded by the BPI as part of the AAP I-Demo.
Additionally, the work was supported by the European Union’s Horizon Europe research and innovation program under Grant Agreement No 101094831 for the Converge-Telecommunications and Computer Vision Convergence Tools for Research Infrastructures project.

