---
layout: page
title: Selected Projects
permalink: /projects/
---

## Vision-Based Proximity Estimation and Haptic Feedback for Surgical Teleoperation

The narrow stereo baseline of surgical endoscopes fundamentally limits depth perception,
increasing cognitive effort during teleoperation. We present a framework that extracts
spatial proximity purely from the stereo endoscopic feed and retargets it to the operator
as directional vibrotactile feedback, supplementing impoverished visual depth cues through
a complementary sensory channel. In a controlled human subject study (n=20), proximity
feedback substantially reduced perceived cognitive workload — particularly frustration,
mental demand, and effort — while maintaining equivalent task performance and accelerating
skill acquisition during training. Perception models were trained on synthetic data
generated from our dVRK digital twin (see below).

<figure>
<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/2xj2fiRlrww" 
  frameborder="0" allowfullscreen>
</iframe>
  <figcaption>Final system including segmentation, depth, contact estimation, and haptic actuation.</figcaption>
</figure>

📄 Galvan, A.F., Rowland, D., and Majewicz Fey, A. Toward vision-based proximity estimation
and tactile feedback for surgical teleoperation. *IEEE RA-L*, 2026. To appear.

---

## Grasp- and Object-Aware Contact Estimation from Vision

An extension of our proximity estimation work addressing its principal failure modes.
By incorporating a geometric model of the surgical instrument and conditioning contact
estimation on inferred grasp state, the pipeline distinguishes between the instrument
approaching an object and the instrument holding one — treating a grasped object as
an extension of the manipulator rather than a contact target. The result is a more
robust contact estimate that remains reliable under occlusion, segmentation noise,
and dynamic grasping conditions.

<iframe width="315" height="560"
  src="https://www.youtube.com/embed/08QSUb7up8w"
  frameborder="0" allowfullscreen>
</iframe>
<iframe width="315" height="560"
  src="https://www.youtube.com/embed/39IcLZFQIW8"
  frameborder="0" allowfullscreen>
</iframe>
<iframe width="315" height="560"
  src="https://www.youtube.com/embed/h2WzMRVDBUo"
  frameborder="0" allowfullscreen>
</iframe>

📄 Galvan, A.F. and Majewicz Fey, A. Grasp- and object-aware contact estimation
from vision. In preparation.

---

## Contact-Based Skill Assessment in Robot-Assisted Surgery

Using proximity estimation from vision, we spatiotemporally cluster contact points
into semantically meaningful contact events and apply statistical methods to derive
metrics that correlate with operator skill. This provides a new and interpretable
way to characterize skill in robot-assisted surgery and, more generally, in teleoperation.

<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/aFxHMmLEPlY" 
  frameborder="0" allowfullscreen>
</iframe>

📄 Galvan, A.F. and Majewicz Fey, A. Characterizing human skill in surgical training using
vision-derived contact. *IEEE RA-L*, 2026. Under review.

---

## dVRK Digital Twin & Synthetic Data Generation

Built a digital twin of the da Vinci Research Kit (dVRK) to support perception model
training for the vision-based contact estimation projects above. Demonstrations were
collected in simulation and expanded using domain randomization over camera pose,
intrinsics, textures, and lighting conditions to improve sim-to-real transfer and
robustness of downstream learned models.

<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/pTjSFg7vM94" 
  frameborder="0" allowfullscreen>
</iframe>

---

## Haptic Teleoperation for Robot Learning

A bilateral teleoperation system developed in collaboration with Sony AI for large-scale
demonstration collection for downstream robot learning. My contributions are the bilateral
teleoperation system between the Lambda.7 haptic feedback device and Roboligent Optimo
and PLATO arm-hand assembly enabling real-time, low-latency control. Moreover I handled
creating a time-aligned data collection framework with HDF5 export, including necessary
calibrations.

<figure>
<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/MCIoHb-zNqw" 
  frameborder="0" allowfullscreen>
</iframe>
  <figcaption>Jenga playing.</figcaption>
</figure>

<figure>
<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/RaPcsjFJJ1s" 
  frameborder="0" allowfullscreen>
</iframe>
  <figcaption>Haptic feedback from sensorized hand.</figcaption>
</figure>

<figure>
<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/MCIoHb-zNqw" 
  frameborder="0" allowfullscreen>
</iframe>
  <figcaption>Real-time block tracking enabled by hand-eye calibration and connection with external perception stack.</figcaption>
</figure>

📄 Dalla Gasperina, S., Kang, D.H., Zhang, H., Galvan, A.F., et al. A bilateral teleoperation
framework for dexterous manipulation. *IEEE RA-P*, 2026. Under review.

📄 Boyea, H., Galvan, A.F., Sentis, L., and Majewicz Fey, A. POVFormer: Learning autonomous
point-of-view control from teleoperated grasping and manipulation demonstrations. *IEEE ROMAN*,
2026. To appear.

---

## Task-Space Retargeting for Dexterous Manipulation in Virtual Environments

A task-space retargeting framework which enables dexterous manipulation
using the Maestro hand exoskeleton. Force feedback is transmitted back
to the user via a joint-space virtual coupling control law.

📄 Galvan, A.F., Ramirez, J.D., Deshpande, A.D., and Majewicz Fey, A. An extended virtual
proxy haptic algorithm for dexterous manipulation in virtual environments. *IEEE WHC*, 2023.