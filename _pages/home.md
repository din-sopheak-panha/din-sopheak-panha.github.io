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

Autonomous mobile robots are robots that can move and work on their own in places such as buildings, factories and roads. To do this, a robot needs to know where it is, plan a path, follow that path accurately and avoid obstacles. When a robot cannot handle a situation alone, a human can drive it remotely through teleoperation, so the human and the robot work together. This is especially hard when the network is slow, because the commands and the camera or sensor data arrive late. My research focuses on navigation, path tracking and shared control teleoperation for mobile robots, tested both in simulation and on real robots. My goal is to build mobile robots that are reliable and safe to work with people in real environments.

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
I am a robotics engineer working in the fields of autonomous mobile robots, path tracking and teleoperation. I received my Engineer’s Degree in Robotics and Automation Engineering from the Institute of Technology of Cambodia in 2026, through the ECAM Engineering double degree program with ECAM LaSalle (France).

I have been a member of the Dynamics and Control Laboratory (DCLab) since 2023, where I built an autonomous indoor food delivery robot for my thesis and a lookahead-based path tracking system for a swerve-drive robot, now under review at RAAI 2026. I also joined Robocon in 2024 with DCLab’s ITC02 team, and in 2025 I led GEE Lab’s ITC01 team while remaining a DCLab member.

My current research focuses on shared control for teleoperated mobile robots under communication delay. I am now looking for a Master’s degree in AI Mobility in Korea, focusing on robot collaboration, autonomous mobile robots and teleoperation.the ECAM Engineering double degree program run by ITC and ECAM LaSalle (France). I have been a member of the Dynamics and Control Laboratory (DCLab) since 2023, where I did my thesis. I joined Robocon in 2024 with DCLab's ITC02 team as an electronics team member, and in 2025 I led GEE Lab's ITC01 team while remaining a DCLab member.

I am now looking for a Master's degree in AI Mobility in Korea, focusing on robot collaboration, autonomous mobile robots and teleoperation.
