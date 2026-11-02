---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(120px, 1fr)); gap: var(--space-3); margin-bottom: var(--space-6);" markdown="0">
<a href="{{ '/projects' | relative_url }}" style="text-align: center; text-decoration: none;">
<img src="https://dinsopheakpanhaportfolio.netlify.app/materials/indoor-delivery-hero.jpg" alt="Autonomous indoor delivery robot" style="width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 8px;" loading="lazy">
<span style="display: block; font-size: 0.8125rem; margin-top: var(--space-2);">Autonomous Mobile Robots</span>
</a>
<a href="{{ '/projects' | relative_url }}" style="text-align: center; text-decoration: none;">
<img src="{{ '/images/robot-arm.jpg' | relative_url }}" alt="Robot arm" style="width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 8px;" loading="lazy">
<span style="display: block; font-size: 0.8125rem; margin-top: var(--space-2);">Robot Arms</span>
</a>
<a href="{{ '/projects' | relative_url }}" style="text-align: center; text-decoration: none;">
<img src="{{ '/images/teleoperation.jpg' | relative_url }}" alt="Teleoperation" style="width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 8px;" loading="lazy">
<span style="display: block; font-size: 0.8125rem; margin-top: var(--space-2);">Teleoperation</span>
</a>
<a href="{{ '/projects' | relative_url }}" style="text-align: center; text-decoration: none;">
<img src="https://dinsopheakpanhaportfolio.netlify.app/materials/swerve-drive-hero.png" alt="Swerve-drive robot" style="width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 8px;" loading="lazy">
<span style="display: block; font-size: 0.8125rem; margin-top: var(--space-2);">Path Tracking</span>
</a>
</div>

My research is on autonomous mobile robots, mainly navigation and path tracking, tested both in simulation and on real robots. At the Dynamics and Control Laboratory (DCLab) at the Institute of Technology of Cambodia, I worked with a teammate to build a fully autonomous indoor food delivery robot using ROS 2 and Nav2, which completed every trial without collisions with a mean position error of about 0.26 m. We built it to explore and research robot navigation systems, inspired by Servi, the restaurant serving robot from Bear Robotics, now majority-owned by LG Electronics. With support from DCLab's Robocon 2025 team, I also designed and integrated a lookahead-based path tracking system for a swerve-drive robot, using ROS 2 and a 3D LiDAR with FAST-LIO2 for localization. I chose this approach because simple PID path tracking on a swerve-drive robot needs separate controllers for x, y and heading, and their gains often have to be retuned for different paths and speeds. In Robocon, our team used PID and had to tune it many times. With the lookahead-based system, the robot followed square, circle and triangle paths with RMS errors between 0.77 and 1.09 cm, using one fixed set of parameters.

I have also worked on robot arms, during my exchange semester in France and in a lab in Cambodia. One of these projects was controlling a robot arm with face tracking using dlib. In industrial automation, I have worked with ABB robot arms, PLCs and HMIs, including a pick-and-place task with an ABB arm and a conveyor sorting system controlled by a PLC and HMI.

I am now working on an independent research project on teleoperated mobile robots under communication delay, in simulation with ROS 2 and Gazebo. Delay has been a real problem for me since I joined Robocon, where our robot lost connection during the competition and could not perform well. I am also interested in teleoperation because it lets a human and a mobile robot work together to do tasks that neither could do well alone. To deal with this problem, I found a paper that motivated me and gave me ideas on how to approach it: "Collision Avoidance with the Novel Advanced Shared Smooth Control in Teleoperated Mobile Robot Vehicles" (Electronics, 2026). Thanks to Dr. Hyun-Rok Cha and his team at KITECH for this work.

## Current work

<div class="section-card" markdown="0">
<ul>
<li><b>Teleoperation under delay:</b> an independent research project on shared control for teleoperated mobile robots under communication delay, in simulation with ROS 2, Gazebo and a 3D LiDAR.</li>
<li><b>Solar tracking system:</b> building a solar tracking system and a management system with the ESP32, supported by STEAMING Cambodia.</li>
</ul>
</div>

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}

## Achievements

<div class="section-card" markdown="0">
<ul>
<li>Cumulative GPA 3.5 / 4.0, Institute of Technology of Cambodia, with 4.0 / 4.0 in academic year 2023-2024</li>
<li>Robocon 2025, Team Leader</li>
<li>Robocon 2024, Electronics Team Member</li>
</ul>
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/achievements' | relative_url }}">All achievements &rarr;</a></p>
</div>

## About me

I am a 2026 graduate of the Institute of Technology of Cambodia, with an Engineer's Degree in Robotics and Automation Engineering from the ECAM Engineering double degree program run by ITC and ECAM LaSalle (France). I have been a member of the Dynamics and Control Laboratory (DCLab) since 2023, where I did my thesis. I joined Robocon in 2024 as an electronics team member and led DCLab's Robocon team in 2025.

I am now looking for a Master's position in Korea in autonomous mobile robots and teleoperation
