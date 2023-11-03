<img src=".\pic.png" style="zoom: 50%;" />

# Description

### Data Acquisition Device

The Artificial Laparoscopic Instrument Dataset (ALID) is a fine-grained labelled dataset acquired on the BellySim lumpectomy simulation training system.

- In order to simulate multi-station clinical training for thoracoscopic and laparoscopic surgery in the form of an artificial pneumoperitoneum, two different stations have been designed.
- The training system consists of trocars, a 30-degree focusable endoscope, a pneumoperitoneum morphology experimental platform, scissors, grasping forceps, and detachment forceps.
 <img src=".\system.png" style="zoom: 50%;" />



### Annotation Process

The ALID dataset was collaboratively overseen by two Medical consultants(one with knowledge of and involvement in laparoscopic surgery and one with a research interest in medical image processing). Annotation was facilitated by six other researchers using *Efficient Interactive Segmentation* ([EISeg](https://github.com/PaddlePaddle/PaddleSeg/tree/release/2.8/EISeg)) toolbox, a high-precision interactive annotation tool. In this case, a frame would be annotated by two annotators and a reviewer would do the initial review and revision. Finally, it was presented to two medical consultants (experts) for final review and revision.



<img src=".\Process.png" style="zoom:50%;" />

### Annotation Status

Each frame is annotated with three categories: background, shaft, and manipulator.

<img src=".\label.png" style="zoom:50%;" />

The ALID dataset contains 1 250 images with the size of 1080 × 1920, involving six scenarios of occlusion, illumination imbalance, category imbalance, smoke, motion artefacts, and blood stains, also including their pair-wise combinations.

Here are the specific settings and collection procedures for the three scenarios:

##### Smoke Simulation:

We use a humidifier to generate a smoke effect, strategically positioning it at various locations. The humidifier operates continuously for one minute, allowing us to capture the smoke's pro-gression from its onset, through even dispersion, to gradual intensification.

##### Blood Stain Simulation:

Artificial blood plasma is used to simulate blood stains. We apply different concentrations of plasma to various parts of the artificial tissue and then move the surgical instruments in con-tact with the tissue to emulate the effect of staining.

##### Motion Artifact Simulation:

Motion artifacts are simulated by rapidly moving the surgical instruments within the camera's field of view. The operator performs a variety of movements at different speeds and directions to capture a range of artifact effects, without the necessity for precise numerical consistency.

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

