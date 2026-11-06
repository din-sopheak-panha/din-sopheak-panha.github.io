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
<img src="{{ '/images/robot-arm.png' | relative_url }}" alt="Robot arm" style="width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 8px;" loading="lazy">
<span style="display: block; font-size: 0.8125rem; margin-top: var(--space-2);">Robot Arms</span>
</a>
<a href="{{ '/projects' | relative_url }}" style="text-align: center; text-decoration: none;">
<img src="{{ '/images/teleoperation.png' | relative_url }}" alt="Face tracking" style="width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 8px;" loading="lazy">
<span style="display: block; font-size: 0.8125rem; margin-top: var(--space-2);">Face Tracking</span>
</a>
<a href="{{ '/projects' | relative_url }}" style="text-align: center; text-decoration: none;">
<img src="https://dinsopheakpanhaportfolio.netlify.app/materials/swerve-drive-hero.png" alt="Swerve-drive robot" style="width: 100%; aspect-ratio: 4 / 3; object-fit: cover; border-radius: 8px;" loading="lazy">
<span style="display: block; font-size: 0.8125rem; margin-top: var(--space-2);">Path Tracking</span>
</a>
</div>

## About me
Hello! I am Din Sopheak Panha, a robotics engineer and a member of the Dynamics and Control Laboratory (DCLab) at the Institute of Technology of Cambodia, currently looking for a Master's degree.

I earned my Engineer's Degree in Robotics and Automation Engineering at the Institute of Technology of Cambodia in 2026, through the ECAM Engineering double degree program with ECAM LaSalle (France), including an exchange semester in France in 2025. During my studies, I built an autonomous indoor food delivery robot for my thesis and a lookahead-based path tracking system for a three-wheel swerve-drive robot.

My research focuses on autonomous mobile robots, with an emphasis on navigation, path tracking and teleoperation. I work on path tracking for holonomic robots, LiDAR-inertial localization with FAST-LIO2, autonomous navigation with Nav2, and shared control for teleoperated mobile robots under communication delay.

My recent work includes lookahead-based path tracking for a three-wheel swerve-drive robot (under review at RAAI 2026) and an autonomous indoor food delivery robot (thesis, 2026). I also led GEE Lab's ITC01 team in ABU Robocon 2025, where we built two robots that could dribble, pass, block, shoot and receive.

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


