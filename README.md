# Robotics_Staubli_UdG_2022

## Introduction
Everyday countless patients enter hospitals in dire need of medical care. On a daily basis the nurses need to sample blood, insert contrast substance or administer intravenous treatment. Due to the considerable number of patients each with their needs, nurses can be overwhelmed and in addition, due to the COVID-19 pandemic, minimizing patient interaction would protect healthcare workers.

## Applicability
Our Staubli TX60 robot is used to move the robotic arm to the nurse to get the needle, slowly move in the direction of the patient’s arm and carefully insert the needle into the vein. The full diagram of the project can be found at a later chapter. Considering the time, we had to fully implement the project and the available logistics, we chose not to use a camera to change the localization of the vein. Instead, we chose to keep a dummy vein at a fixed position to simulate a human arm with a vein and use the fully calibrated robotic arm to move in a frame we defined towards the vein.
We took into account the anatomical accuracy of the insertion and we selected the angle to be of 10-15 degrees. We give the choice to the user to choose between 3 initial speed levels and as we go closer to the vein, we significantly slow down the speed. This is meant to reduce the impact to the skin and avoid bruising, have move control on the movement and minimize the potential surprise and worry the patient might have since the population is not yet used to robotic interaction. In a symmetric way, we retract the needle and the it reaches the home position with the same speed checkpoints, but in reversed order.


