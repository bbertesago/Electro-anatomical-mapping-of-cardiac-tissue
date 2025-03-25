# Electro-anatomical-mapping-of-cardiac-tissue
Atrial arrhythmias, including atrial fibrillation, are a major global health problem; the latter was estimated to affect 7.6 million people over 65 in the EU in 2016.
The data used in this project comes from electro-anatomical maps, which help clinicians to understand the movement of cardiac tissue during electrical impulses.
The project is divided into 3 checkpoints.\
**1st Checkpoint**: The task is to adopt a fully data-driven approach to reconstruct activation time and conduction velocity from sparse measurements over the entire domain. The intended strategy to be used is interpolation, specifically radial basis functions (RBF).\
**2nd Checkpoint**: The second task is to determine an estimate of an unknown parameter vector μ, containing three patient-specific quantities: fiber angle, anisotropy ratio and shock wave starting point. The physical law (Eikonal equation) to which the model is subject is introduced, considering the conduction velocity as a constant. Given the presence of a physical constraint to be satisfied, a Physics-Informed Neural-Network (PINN) is employed.\
**3rd Checkpoint**: The last checkpoint is an extension of the previous one. The goal is to reconstruc the velocity field for a patient, given his twenty measurements and the estimates of the field for a hundred patients.

For more details check the uploaded report **Report_p1**.
