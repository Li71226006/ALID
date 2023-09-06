<img src=".\pic.png" style="zoom: 50%;" />

### Description

The Artificial Laparoscopic Instrument Dataset (ALID) is a fine-grained labelled dataset acquired on the BellySim lumpectomy

 simulation training system.
- In order to simulate multi-station clinical training for thoracoscopic and laparoscopic surgery in the form of an artificial pneumoperitoneum, two different stations have been designed.
- The training system consists of trocars, a 30-degree focusable endoscope, a pneumoperitoneum morphology experimental platform, scissors, grasping forceps, and detachment forceps.
 <img src=".\system.png" style="zoom: 50%;" />



- The ALID dataset contains 1 250 images with the size of 1080 × 1920, involving six scenarios of occlusion, illumination imbalance, category imbalance, smoke, motion artefacts, and blood stains, also including their pair-wise combinations.

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

