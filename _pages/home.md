---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Autonomous Mobile Robots</a>
<a href="{{ '/research' | relative_url }}" class="chip">Robot Arms</a>
<a href="{{ '/research' | relative_url }}" class="chip">Teleoperation</a>
<a href="{{ '/research' | relative_url }}" class="chip">Path Tracking</a>
</div>

My research focuses on autonomous mobile robots, with particular emphasis on navigation and path tracking, validated both in simulation and on physical hardware. In collaboration with a teammate, I developed a fully autonomous indoor food delivery robot based on ROS 2 and the Nav2 navigation framework. Independently, I developed a path tracking algorithm for a swerve-drive robot, using ROS 2 and a 3D LiDAR with FAST-LIO2 for localization.

My work also extends to robotic manipulation. During an exchange semester in France and in a laboratory in Cambodia, I worked on robot arm projects, including face tracking control of a robot arm using dlib. In industrial automation, I have experience with ABB industrial robot arms, PLCs and HMIs, including a pick-and-place task with an ABB robot arm and a conveyor-based sorting system controlled by a PLC and HMI.

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

I am a graduate of the Department of Industrial and Mechanical Engineering at the Institute of Technology of Cambodia, where I completed the Engineer's Degree in Robotics and Automation Engineering in 2026 through the ECAM Engineering international double degree program, delivered by ITC and ECAM LaSalle (France). My thesis focused on the development of an autonomous indoor food delivery robot. In addition to my research, I have worked as a robotics tutor at Seksaa Tech Academy and STEAMING Cambodia. I am currently seeking a Master's position in Korea in the field of autonomous mobile robots and teleoperation.
