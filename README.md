<img src=".\pic.png" style="zoom: 50%;" />

# Description

### Data Acquisition Device

The Artificial Laparoscopic Instrument Dataset (ALID) is a fine-grained labelled dataset acquired on the BellySim lumpectomy simulation training system.

- In order to simulate multi-station clinical training for thoracoscopic and laparoscopic surgery in the form of an artificial pneumoperitoneum, two different stations have been designed.
- The training system consists of trocars, a 30-degree focusable endoscope, a pneumoperitoneum morphology experimental platform, scissors, grasping forceps, and detachment forceps.
 <img src=".\system.png" style="zoom: 50%;" />



### Annotation Process

The ALID dataset was collaboratively overseen by two medical students(one with knowledge of and involvement in laparoscopic surgery and one with a research interest in medical image processing). Annotation was facilitated by six other researchers using *Efficient Interactive Segmentation* ([EISeg](https://github.com/PaddlePaddle/PaddleSeg/tree/release/2.8/EISeg)) toolbox, a high-precision interactive annotation tool. In this case, a frame would be annotated by two annotators and a reviewer would do the initial review and revision. Finally, it was presented to two medical students (experts) for final review and revision.



<img src=".\Process.png" style="zoom:50%;" />

### Annotation Status

Each frame is annotated with three categories: background, shaft, and manipulator.

<img src=".\label.png" style="zoom:50%;" />

The ALID dataset contains 1 250 images with the size of 1080 × 1920, involving six scenarios of occlusion, illumination imbalance, category imbalance, smoke, motion artefacts, and blood stains, also including their pair-wise combinations.

Here are the specific settings and collection procedures for the three scenarios:

##### Smoke Simulation:

We utilize a humidifier to generate a smoke effect. The humidifier is strategically positioned at various locations and operates continuously for 1 minute. This approach captures the progression of smoke, from its onset to even dispersion and its gradual intensification.

##### Blood Stain Simulation:

Artificial blood plasma is employed to simulate blood stains. We smear different concentrations of the plasma on varied parts of the artificial tissue. Then, by moving the surgical instruments in contact with the tissue, we emulate the effect of instruments becoming stained.

##### Motion Artifact Simulation:

Motion artifacts are simulated by swiftly moving the surgical instruments within the camera's viewing window. To encapsulate a range of artifact effects, the operator attempts various movement directions and speeds, without the need for precise numerical consistency.

<img src=".\classes.png" style="zoom:25%;" />

The corresponding number of categories is as follows:

|          Category          | Normal  | Occlusion | Smoke  | Blood Stains | Category Imbalance | Illumination Imbalance | Motion Artifacts |
| :------------------------: | :-----: | :-------: | :----: | :----------: | :----------------: | :--------------------: | :--------------: |
|         **Normal**         | **150** |  **120**  | **60** |    **60**    |      **130**       |        **120**         |      **60**      |
|       **Occlusion**        |  **-**  |   **-**   | **20** |    **20**    |       **60**       |         **60**         |      **60**      |
|         **Smoke**          |  **-**  |   **-**   | **-**  |    **30**    |       **20**       |         **20**         |      **20**      |
|      **Blood Stains**      |  **-**  |   **-**   | **-**  |    **-**     |       **20**       |         **20**         |      **20**      |
|   **Category Imbalance**   |  **-**  |   **-**   | **-**  |    **-**     |       **-**        |         **60**         |      **60**      |
| **Illumination Imbalance** |  **-**  |   **-**   | **-**  |    **-**     |       **-**        |         **-**          |      **60**      |

### Contact

For more information and access to datasets please contact us
(wangzhengyu_hfut@hfut.edu.cn)

