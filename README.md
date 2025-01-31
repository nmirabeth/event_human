# Human-centered applications of event data 

This is the official repository of "Event-based solutions for human-centered applications: A comprehensive review" submitted to Frontiers in Signal Processing journal.

Event cameras, or dynamic vision sensors, capture changes in light intensity asynchronously, providing high temporal resolution and energy efficiency. These features make them ideal for human-centered applications, such as analyzing facial expressions and body motion dynamics. However, research in this area is fragmented. This repository unifies advancements in body and face-related tasks, offering a comprehensive review of databases, event data representation, and processing models. It serves as a foundational resource for researchers, guiding future work in human-centered event camera applications.

# Datasets

## Real event-based datasets for human-centered applications
### Body Datasets

| Year | Authors | Name | #Videos | #People | Modalities | Application | #Classes |
|------|---------|------|------------|----------|------------|-------------|-----------|
| 2019 | [Miao et al. (2019)](#miao2019) | Action Dataset TUM | 291 | 15 | EV | Action Recognition | 10
| 2019 | [Calabrese et al. (2019)](#calabrese2019) | DHP19 | 2244 | 17 | EV | Pose Estimation | -
| 2019 | [Wang et al. (2019)](#wang2019) | DVS128-Gait-Day | 4000 | 20 | EV | Gait Recognition | -
| 2019 | [Wang et al. (2019)](#wang2019) | DVS128-Gait-Night | 4000 | 20 | EV | Gait Recognition | -
| 2021 | [Liu et al. (2021)](#liu2021) | DailyAction-DVS | 1440 | 15 | EV | Action Recognition | 12
| 2022 | [Eddine and Dugelay (2022)](#dugelay2022) | Gait3 | 168 | 56 | RGB-EV-TH | Gait Recognition | -
| 2023 | [Gao et al. (2023)](#gao2023) | THU-E-ACT-50 | 10500 | 105 | EV | Action Recognition | 50
| 2023 | [Gao et al. (2023)](#gao2023)| THU-E-ACT-50-CHL | 2330 | 18 | EV | Action Recognition | 50
| 2024 | [Gao et al. (2024)](#gao2024) | THU-MV-E-ACT-50 | 31500 | 105 | EV | Action Recognition | 50
| 2025 | [Wang et al. (2025)](#wang2025) | DailyDVS-200 | 22000 | 46 | RGB-EV | Action Recognition | 200


### Face Datasets

| Year | Authors | Name | #Videos | #People | Modalities | Application |
|------|---------|------|------------|----------|------------|-------------|
| 2016 | [Barua et al. (2016)](#barua2016) | - | - | 40 | EV | Face Detection 
| 2019 | [Li et al. (2019)](#li2019) | - | 34000 | 34 | EV-audio | Lip Reading 
| 2020 | [Angelopoulos et al. (2020)](#angelopoulos2020) | - | 24 | 24 | EV | Eye gaze tracking
| 2020 | [Chen et al. (2020a)](#chen2020a) | EDDD | 260 | 26 | EV | Drowsiness 
| 2020 | [Lenz et al. (2020)](#lenz2020) | - | 48 | 10 | EV | Face Detection 
| 2020 | [Chen et al. (2020b)](#chen2020b) | NeuroBiometric | 180 | 45 | EV | Authentication 
| 2022 | [Banerjee et al. (2022)](#banerjee2022) | - | 3360 | 6 | RGB-EV | Eye gaze tracking
| 2022 | [Beccattini et al. (2022)](#beccattini2022) | - | 455 | 25 | RGB-EV | MER 
| 2022 | [Tan et al. (2022)](#tan2022) | DVS-Lip | 19871 | 40 | EV | Lip Reading 
| 2022 | [Moreira et al. (2022)](#moreira2022) | NVSFD | 436 | 40 | EV | Identity Recognition 
| 2023 | [Bissarinova et al. (2023)](#bissa2023) | FES | ∼4000 | 73 | EV | Face Detection 
| 2023 | [Berlincioni et al. (2023)](#berlincioni2023) | NEFER | 29 | 105 | RGB-EV | MER 
| 2023 | [Kanamaru et al. (2023)](#kanamaru2023) | - | 1500 | 20 | EV | Lip Reading 
| 2024 | [Adra et al. (2024)](#adra2024b) | VETEX | 2506 | 30 | RGB-EV-TH | MER


## Synthetic datasets for human-centered applications
### Body Datasets

| Year | Authors | Name | #Videos | #People | Application | #Classes |
|------|---------|------|---------|---------|-------------|----------|
| 2019 | [Wang et al. (2019)](#wang2019)| EV-CASIA-B | 8184 | 124 | Gait Recognition | -
| 2020 | [Bi et al. (2020)](#bi2020) | HMDB51-DVS | 6766 | - | Action Recognition | 51
| 2020 | [Bi et al. (2020)](#bi2020) | UCF101-DVS | 13320 | - | Action Recognition | 101
| 2022 | [Plizzari et al. (2022)](#plizzari2022) | N-EPIC-Kitchens | 64 | - | Action Recognition | 8
| 2023 | [Zou et al. (2023)](#zou2023) | SynEventHPD | 9197 | 47 | Pose Estimation | -
| 2023 | [Goyal et al. (2023)](#goyal2023) | eH36m | 748 | 7 | Pose Estimation | -


### Face Datasets

| Year | Authors | Name | #Videos | #People | Application |
|------|---------|------|------------|----------|---------|
| 2022 | [Moreira et al. (2022)](#moreira2022)| SynFED | 6536 | 30 | Identity Recognition 
| 2023 | [Barchid et al. (2023)](#barchid2023) | ADFES | 198 | 22 | Face Expression Recognition
| 2023 | [Barchid et al. (2023)](#barchid2023) | Oulu-CASIA | 480 | 80 | Face Expression Recognition
| 2023 | [Barchid et al. (2023)](#barchid2023) ; [Verschae and Bugueno-Cordova (2023)](#verschae2023) | e-CK+ | 327 | 93 | Face Expression Recognition
| 2023 | [Barchid et al. (2023)](#barchid2023) ; [Verschae and Bugueno-Cordova (2023)](#verschae2023) |e-MMI | 2900+ | 75 | Face Expression Recognition
| 2023 | [Ryan et al. (2023)](#ryan2023) | - | - | 5 | Multitask Facial Analysis
| 2024 | [Tan et al. (2024)](#tan2024) | DVS-LRW100 | 107664 | - | Lip Reading

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

| SNN                          | Graph NN                     | CNN                          | Transformers                 | Not AI-based                 |
|------------------------------|------------------------------|------------------------------|------------------------------|------------------------------|
| [Liu et al. (2021)](#liu2021)            | [Wang et al. (2021)](#wang2021)     | [Li et al. (2019)](#li2019)                   | [Xu et al. (2020)](#xu2020)                  | [Barua et al. (2016)](#barua2016) 
| [Barchid et al. (2023)](#barchid2023)    | [Eisl et al. (2023)](#eisl2023)     | [Wang et al. (2019)](#wang2019)               | [de Blegiers et al. (2023)](#deblegiers2023) | [Savran et al. (2018)](#savran2018)
| [Ren et al. (2023b)](#ren2023b)            | [Fu and Yan (2023)](#fun2023)       | [Sokolova and Konushin (2019)](#sokolova2019) | [Zou et al. (2023)](#zou2023)                | [Lenz et al. (2020)](#lenz2020)
| [Bulzomi et al. (2023)](#bulzomi2023)        | [Gao et al. (2024)](#gao2024)       | [Ryan et al. (2021)](#ryan2021)               | [Cultrera et al. (2023)](#cultrera2024)      | [Chen et al. (2020b)](#chen2020b)
| [Tao et al. (2024)](#tao2024)           |                                     | [Banerjee et al. (2022)](#banerjee2022)       |                                              | [Angelopoulos et al. (2020)](#angel2020)             
| [Vicente-Sola et al. (2025)](#vicente2025)   |                                     | [Becattini et al. (2022)](#becattini2022)     |                                              | [Eddine and Dugelay (2022)](#dugelay2022)           
|                                          |                                     | [Moreira et al. (2022)](#moreira2022)         |                                              | [Ren et al. (2023a)](#ren2023a) 
|                                          |                                     | [Plizzari et al. (2022)](#plizzari2022)       |                                              | [Guo and Huang (2023)](#hang2023)            
|                                          |                                     | [Ryan et al. (2023)](#ryan2023)               |                                              | [Savran (2023)](#savran2023)            
|                                          |                                     | [Gao et al. (2023)](#gao2023)                 |                                              | [Himmi et al. (2024)](#himmi2024)  
|                                          |                                     | [Rios-Navarro et al. (2023)](#rios2023)       |                                              | 
|                                          |                                     | [Bissarinova et al. (2023)](#bissa2023)       |                                              | 
|                                          |                                     | [Berlincioni et al. (2023)](#berlin2023)      |                                              | 
|                                          |                                     | [Goyal et al. (2023)](#goyal2023)             |                                              | 
|                                          |                                     | [Kanamaru et al. (2023)](#kanamaru2023)       |                                              | 
|                                          |                                     | [Xiao et al. (2024)](#xiao2024)               |                                              | 
|                                          |                                     | [Kohyama et al. (2024)](#kohyama2024)         |                                              | 
|                                          |                                     | [Adra et al. (2024)](#adra2024)               |                                              | 
|                                          |                                     | [Iddrisu et al. (2024)](#iddrisu2024)         |                                              | 



# Applications

### Applications of event cameras for human data along with an exhaustive selection of relevant work

### Body

| Human Tracking | Gait Recognition | Action Recognition | Pose Estimation |
|------------------------------------------|-------------------------------------|-----------------------------------------------|------------------------------|
| [Eisl et al. (2023)](#eisl2023)          | [Wang et al. (2021)](#wang2021)                  | [Liu et al. (2021)](#liu2021)                    | [Sokolova and Konushin (2019)](#sokolova2019)               
| [Xu et al. (2020)](#xu2020)              | [Sokolova and Konushin (2019)](#sokolova2019)     | [Plizzari et al. (2022)](#plizzari2022)          | [Zou et al. (2023)](#zou2023)   
|                                          | [Wang et al. (2021)](#wang2021)                  | [Ren et al. (2023a)](#ren2023a)                  | [Goyal et al. (2023)](#goyal2023)  
|                                          | [Eddine and Dugelay (2022)](#dugelay2022)        | [Ren et al. (2023b)](#ren2023b)                  | [Kohyama et al. (2024)](#kohyama2024)       
|                                          | [Fu and Yan (2023)](#fun2023)                    | [de Blegiers et al. (2023)](#deblegiers2023)     |                                                  
|                                          | [Tao et al. (2024)](#tao2024)                    | [Gao et al. (2023)](#gao2023)                    |                                                   
|                                          |                                                  | [Gao et al. (2024)](#gao2024)                    |                                              
|                                          |                                                  | [Vicente-Sola et al. (2025)](#vicente2025)       |                                                     
|                                          |                                                  | [Wang et al. (2025)](#wang2025)                  |                                                  
                 


### Face

| Face Detection | Identity Recognition | Lip Reading | Eye Blinking & Gaze | Microexpression & Emotion Recognition |
|------------------------------------------|-------------------------------------|-----------------------------------------------|----------------------------------------------|------------------------------|
| [Barua et al. (2016)](#barua2016)        | [Chen et al. (2020b)](#chen2020b)     | [Savran et al. (2018)](#savran2018)           | [Lenz et al. (2020)](#lenz2020)              | [Beccatini et al. (2022)](#beccatini2022) 
| [Lenz et al. (2020)](#lenz2020)          | [Moreira et al. (2022)](#moreira2022) | [Li et al. (2019)](#li2019)                   | [Chen et al. (2020b)](#chen2020b)            | [Barchid et al. (2023)](#barchid2023) 
| [Ryan et al. (2021)](#ryan2021)          |                                       | [Rios-Navarro et al. (2023)](#rios2023)       | [Angelopoulos et al. (2020)](#angel2020)     | [Berlincioni et al. (2023)](#berlin2023)
| [Bissarinova et al. (2023)](#bissa2023)  |                                       | [Savran (2023)](#savran2023)                  | [Ryan et al. (2021)](#ryan2021)              | [Guo and Huang (2023)](#hang2023)    
| [Ryan et al. (2023)](#ryan2023)          |                                       | [Kanamaru et al. (2023)](#kanamaru2023)       | [Banerjee et al. (2022)](#banerjee2022)      | [Xiao et al. (2024)](#xiao2024)          
| [Himmi et al. (2024)](#himmi2024)        |                                       | [Bulzomi et al. (2023)](#bulzomi2023)         | [Iddrisu et al. (2024)](#iddrisu2024)         | [Cultrera et al. (2023)](#cultrera2024)        
| [Iddrisu et al. (2024)](#iddrisu2024b)     |                                       | [Moreira et al. (2022)](#moreira2022)         |                                              | [Adra et al. (2024)](#adra2024b)  



# Event-RGB comparison

### Summary of the works included in this survey that compare their event-based networks with RGB-trained models. 

| Target Application                  | Authors & Year                    | Findings | Improvements of Event |
|--------------------------------------|------------------------------------|----------|-----------------------|
| **Gait Recognition**                 | [Wang et al. (2019)](#wang2019)    | For viewing angles 72, 90, and 108, EV-Gait performs better than RGB-based approaches | 3% increase in accuracy |
|                                      | [Sokolova and Konushin (2019)](#sokolova2019)      | Similar performances reported for Event-based and RGB approaches | - |
|                                      | [Wang et al. (2021)](#wang2021)                | For viewing angle 90 degrees, EV-Gait-Graph performs better than RGB-based approaches | 0.5% increase in accuracy |
|                                      | [Eddine and Dugelay (2022)](#dugelay2022)         | Advantage of event data over RGB and thermal for gait recognition | 2% increase in accuracy |
|                                      | [Tao et al. (2024)](#tao2024)                 | They report the advantage of event over RGB across all different rotation angles for gait recognition | Up to 14% increase in accuracy |
| **Action Recognition**               | [Plizzari et al. (2022)](#plizzari2022)             | Event data can surpass RGB for action recognition in unseen scenarios on test data | 4% increase in accuracy |
|                                      | [de Blegiers et al. (2023)](#deblegiers2023)          | Event surpasses RGB action recognition models in different setups | Up to 14% increase in accuracy |
| **Pose Estimation**                  | [Goyal et al. (2023)](#goyal2023)                | Pose estimation from event data surpasses RGB data | Up to 5% increase in accuracy |
|                                      | [Kohyama et al. (2024)](#kohyama2024)              | Event does not suffer from motion blur as RGB does for 3D-based pose estimation | Error (in mm) is divided by 5 in certain scenarios |
| **Face Detection**                   | [Barua et al. (2016)](#barua2016)                | Comparable results to Viola-Jones face detector | - |
|                                      | [Ryan et al. (2023)](#ryan2023)                 | Traditional RGB models perform better on RGB images than on their simulated event data counterpart | - |
| **Lip Reading**                      | [Kanamaru et al. (2023)](#kanamaru2023)             | They combined event and RGB modalities for lip reading | - |
| **Microexpression & Emotion Recognition** | [Becattini et al. (2022)](#becattini2022)       | Event data outperforms RGB for detecting three types of expressions: Positive, Neutral, Negative | Up to 9% increase in accuracy |
|                                      | [Berlincioni et al. (2023)](#berlincioni2023)          | Event performs better than RGB in emotion recognition | Up to 15% increase in accuracy |
|                                      | [Xiao et al. (2024)](#xiao2024)                 | Event and RGB are fused to the network | 1% increase in accuracy |
|                                      | [Cultrera et al. (2024)](#cultrera2024)              | For the first time, results on event data deliver better performance | For 6 out of 24 action units, event data is more accurate |
|                                      | [Adra et al. (2024)](#adra2024b)                | Event data gives higher recognition than RGB | Up to 13% increase in accuracy |



## Bibliography

- <a id="miao2019"></a> Miao, S., Chen, G., Ning, X., Zi, Y., Ren, K., Bing, Z., et al. (2019). Neuromorphic vision datasets for pedestrian detection, action recognition, and fall detection
- <a id="calabrese2019"></a> Calabrese, E., Taverni, G., Easthope, C. A., Skriabine, S., Corradi, F., Longinotti, L., et al. (2019). Dhp19: Dynamic vision sensor 3d human pose dataset
- <a id="wang2019"></a> Wang, Y., Du, B., Shen, Y., Wu, K., Zhao, G., Sun, J., et al. (2019). Ev-gait: Event-based robust gait recognition using dynamic vision sensors
- <a id="wang2021"></a> Wang, Y., Zhang, X., Shen, Y., Du, B., Zhao, G., Cui, L., et al. (2021). Event-stream representation for human gaits identification using deep neural networks (IEEE), vol. 44, 3436–3449
- <a id="dugelay2022"></a> Eddine, M. J. and Dugelay, J.-L. (2022). Gait3: An event-based, visible and thermal database for gait recognition
- <a id="liu2021"></a> Liu, Q., Xing, D., Tang, H., Ma, D., and Pan, G. (2021). Event-based action recognition using motion information and spiking neural networks.
- <a id="gao2023"></a> Gao, Y., Lu, J., Li, S., Ma, N., Du, S., Li, Y., et al. (2023). Action recognition and benchmark
using event cameras
- <a id="gao2024"></a> Gao, Y., Lu, J., Li, S., Li, Y., and Du, S. (2024). Hypergraph-based multi-view action recognition using event cameras
- <a id="wang2025"></a> Wang, Q., Xu, Z., Lin, Y., Ye, J., Li, H., Zhu, G., et al. (2025). Dailydvs-200: A comprehensive
benchmark dataset for event-based action recognition
- <a id="angelopoulos2020"></a> Angelopoulos, A. N., Martel, J. N., Kohli, A. P., Conradt, J., and Wetzstein, G. (2020). Event-based near-eye gaze tracking beyond 10,000 hz
- <a id="chen2020a"></a> Chen, G., Hong, L., Dong, J., Liu, P., Conradt, J., and Knoll, A. (2020a). Eddd: Event-based
drowsiness driving detection through facial motion analysis with neuromorphic vision sensor
- <a id="chen2020b"></a> Chen, G., Wang, F., Yuan, X., Li, Z., Liang, Z., and Knoll, A. (2020b). Neurobiometric: an eye blink based biometric authentication system using an event-based neuromorphic vision sensor
- <a id="tan2022"></a> Tan, G., Wang, Y., Han, H., Cao, Y., Wu, F., and Zha, Z. J. (2022). Multi-grained spatio-temporal features perceived network for event-based lip-reading
- <a id="tan2024"></a> Tan, G., Wan, Z., Wang, Y., Cao, Y., and Zha, Z. J. (2024). Tackling event-based lip-reading by exploring multigrained spatiotemporal clues. IEEE Transactions on Neural Networks and Learning Systems
- <a id="bissa2023"></a> Bissarinova, U., Rakhimzhanova, T., Kenzhebalin, D., and Varol, H. A. (2023). Faces in event streams(fes): An annotated face dataset for event cameras (Authorea)
- <a id="berlincioni2023"></a> Berlincioni, L., Cultrera, L., Albisani, C., Cresti, L., Leonardo, A., Picchioni, S., et al. (2023).Neuromorphic event-based facial expression recognition
- <a id="kanamaru2023"></a> Kanamaru, T., Arakane, T., and Saitoh, T. (2023). Isolated single sound lip-reading using a
frame-based camera and event-based camera
- <a id="adra2024b"></a> Adra, M., Mirabet-Herranz, N., and Dugelay, J.-L. (2024). Beyond rgb: Tri-modal
microexpression recognition with rgb, thermal, and event data
- <a id="bi2020"></a> Bi, Y., Chadha, A., Abbas, A., Bourtsoulatze, E., and Andreopoulos, Y. (2020). Graph-based
spatio-temporal feature learning for neuromorphic vision sensing
- <a id="plizzari2022"></a> Plizzari, C., Planamente, M., Goletto, G., Cannici, M., Gusso, E., Matteucci, M., et al. (2022).
E2 (go) motion: Motion augmented event stream for egocentric action recognition
- <a id="zou2023"></a> Zou, S., Mu, Y., Zuo, X., Wang, S., and Cheng, L. (2023). Event-based human pose tracking by spiking spatiotemporal transformer
- <a id="goyal2023"></a> Goyal, G., Di Pietro, F., Carissimi, N., Glover, A., and Bartolozzi, C. (2023). Moveenet: Online
high-frequency human pose estimation with an event camera
- <a id="verschae2023"></a> Verschae, R. and Bugueno-Cordova, I. (2023). Event-based gesture and facial expression
recognition: A comparative analysis
- <a id="ryan2023"></a> Ryan, C., Elrasad, A., Shariff, W., Lemley, J., Kielty, P., Hurney, P., et al. (2023). Real-time multi-task facial analytics with event cameras. IEEE Access
- <a id="ren2023a"></a> Ren, H., Zhou, Y., Fu, H., Huang, Y., Xu, R., and Cheng, B. (2023a). Ttpoint: A tensorized point
cloud network for lightweight action recognition with event cameras. In Proceedings of the 31st ACM International Conference on Multimedia. 8026–8034
- <a id="ren2023b"></a> Ren, H., Zhou, Y., Huang, Y., Fu, H., Lin, X., Song, J., et al. (2023b). Spikepoint: An efficient point-based spiking neural network for event cameras action recognition. arXiv preprint arXiv:2310.07189
- <a id="bulzomi2023"></a> Bulzomi, H., Schweiker, M., Gruel, A., and Martinet, J. (2023). End-to-end neuromorphic lip-reading. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 4101–4108
- <a id="vicente2025"></a> Vicente-Sola, A., Manna, D. L., Kirkland, P., Di Caterina, G., and Bihl, T. J. (2025). Spiking neural networks for event-based action recognition: A new task to understand their advantage. Neurocomputing 611, 128657
- <a id="eisl2023"></a> Eisl, D., Herzog, F., Dugelay, J.-L., Apvrille, L., and Rigoll, G. (2023). Introducing a framework for single-human tracking using event-based cameras. In 2023 IEEE International Conference on Image Processing (ICIP) (IEEE), 3269–3273
- <a id="fu2023"></a> Fu, L. and Yan, S. (2023). Hypergraph neural network for gait recognition based on event camera. In Third International Conference on Advanced Algorithms and Signal Image Processing (AASIP 2023) (SPIE), vol. 12799, 1151–1155
- <a id="tan2022"></a> Tan, G., Wang, Y., Han, H., Cao, Y., Wu, F., and Zha, Z. J. (2022). Multi-grained spatio-temporal features perceived network for event-based lip-reading
- <a id="rios2023"></a> Rios-Navarro, A., Pi ˜nero-Fuentes, E., Canas-Moreno, S., Javed, A., Harkin, J., and Linares-Barranco, A.(2023). Lipsfus: A neuromorphic dataset for audio-visual sensory fusion of lip reading. In 2023 IEEE
International Symposium on Circuits and Systems (ISCAS) (IEEE), 1–5
- <a id="xiao2024"></a> Xiao, P., Zhang, Y., Kai, D., Peng, Y., Zhang, Z., and Sun, X. (2024). Estme: Event-driven spatio-temporal motion enhancement for micro-expression recognition. In 2024 IEEE International Conference on Multimedia and Expo (ICME) (IEEE), 1–6
- <a id="kohyama2024"></a> Kohyama, K., Shiba, S., and Aoki, Y. (2024). 3d human scan with a moving event camera. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 5586–5596
- <a id="iddrisu2024b"></a> Iddrisu, K., Shariff, W., OConnor, N. E., Lemley, J., and Little, S. (2024). Evaluating
image-based face and eye tracking with event cameras
- <a id="deblegiers2023"></a> de Blegiers, T., Dave, I. R., Yousaf, A., and Shah, M. (2023). Eventtransact: A video transformer-based framework for event-camera based action recognition. In 2023 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) (IEEE), 1–7
- <a id="cultrera2024"></a> Cultrera, L., Becattini, F., Berlincioni, L., Ferrari, C., and Del Bimbo, A. (2024). Spatio-temporal transformers for action unit classification with event cameras. arXiv preprint arXiv:2410.21958
- <a id="guo2023"></a> Guo, C. and Huang, H. (2023). Gleffn: A global-local event feature fusion network for micro-expression recognition. In Proceedings of the 3rd Workshop on Facial Micro-Expression: Advanced Techniques for
Multi-Modal Facial Expression Analysis. 17–24
- <a id="savran2023"></a> Savran, A. (2023). Fully convolutional event-camera voice activity detection based on event intensity. In 2023 Innovations in Intelligent Systems and Applications Conference (ASYU) (IEEE), 1–6
- <a id="himmi2024"></a> Himmi, S., Parret, V., Chhatkuli, A., and Van Gool, L. (2024). Ms-evs: Multispectral event-based vision for deep learning based face detection. In Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision. 616–625
- <a id="tao2024"></a> Tao, Y., Chang, C.-H., Sa¨ıghi, S., and Gao, S. (2024). Gaitspike: Event-based gait recognition with spiking neural network. In 2024 IEEE 6th International Conference on AI Circuits and Systems (AICAS) (IEEE), 357–361
- <a id="barchid2023"></a> Barchid, S., Allaert, B., Aissaoui, A., Mennesson, J., and Djeraba, C. C. (2023). Spiking-fer: Spiking neural network for facial expression recognition with event cameras. In 20th International Conference on Content-based Multimedia Indexing. 1–7. doi:10.1145/3617233.3617235
- <a id="li2019"></a> Li, X., Neil, D., Delbruck, T., and Liu, S.-C. (2019). Lip reading deep network exploiting multi-modal spiking visual and auditory sensors
- <a id="xu2020"></a> Xu, L., Xu, W., Golyanik, V., Habermann, M., Fang, L., and Theobalt, C. (2020). Eventcap: Monocular 3d capture of high-speed human motions using an event camera. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. 4968–4978
- <a id="barua2016"></a> Barua, S., Miyatani, Y., and Veeraraghavan, A. (2016). Direct face detection and video
reconstruction from event cameras
- <a id="savran2018"></a> Savran, A., Tavarone, R., Higy, B., Badino, L., and Bartolozzi, C. (2018). Energy and computation
efficient audio-visual voice activity detection driven by event-cameras. In 2018 13th IEEE International Conference on Automatic Face & Gesture Recognition (FG 2018) (IEEE), 333–340
- <a id="lenz2020"></a> Lenz, G., Ieng, S.-H., and Benosman, R. (2020). Event-based face detection and tracking using
the dynamics of eye blinks
- <a id="sokolova2019"></a> Sokolova, A. and Konushin, A. (2019). Human identification by gait from event-based camera. In 2019 16th International Conference on Machine Vision Applications (MVA) (IEEE), 1–6
- <a id="ryan2021"></a> Ryan, C., O’Sullivan, B., Elrasad, A., Cahill, A., Lemley, J., Kielty, P., et al. (2021). Real-time face & eye tracking and blink detection using event cameras. Neural Networks 141, 87–97
- <a id="banerjee2022"></a> Banerjee, A., Prasad, S. S., Mehta, N. K., Kumar, H., Saurav, S., and Singh, S. (2022). Gaze
detection using encoded retinomorphic events
- <a id="becattini2022"></a> Becattini, F., Palai, F., and Bimbo, A. D. (2022). Understanding human reactions looking at
facial microexpressions with an event camera. doi:10.1109/TII.2022.3195063
- <a id="moreira2022"></a> Moreira, G., Grac¸ a, A., Silva, B., Martins, P., and Batista, J. (2022). Neuromorphic event-based face identity recognition


# Acknowledgement

This research is a part of the HEIMDALL project, funded by the BPI as part of the AAP I-Demo.
Additionally, the work was supported by the European Union’s Horizon Europe research and innovation program under Grant Agreement No 101094831 for the Converge-Telecommunications and Computer Vision Convergence Tools for Research Infrastructures project.

