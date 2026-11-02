 ---
title: "Projects"
layout: page
permalink: /projects/
---

# Projects

## Mobile Robots

<div class="section-card" markdown="0">
<h3>Lookahead-Based Path Tracking for a Three-Wheel Swerve-Drive Robot</h3>
<p class="text-muted">DCLab, Institute of Technology of Cambodia · 2025 · ROS 2, C++, Livox Mid-360, FAST-LIO2, CAN bus</p>
<p>PID path tracking on a swerve-drive robot needs separate controllers for x, y and heading, and the gains have to be retuned for different paths. I designed and integrated a lookahead-based path tracking system that projects the robot pose onto the path, looks ahead a fixed distance and computes the velocity command directly, with speed scheduled from path curvature. It runs at 100 Hz, sends commands to three motor drivers over CAN bus, and uses the Livox Mid-360 with FAST-LIO2 for localization.</p>
<ul>
<li>RMS cross-track error of 0.77, 0.80, 1.09 and 2.89 cm on square, circle, triangle and star paths, at up to 1.5 m/s.</li>
<li>One fixed set of parameters for all four paths, with no retuning.</li>
<li>Paper under review at RAAI 2026.</li>
</ul>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: var(--space-4); margin-top: var(--space-4);">
<img src="https://dinsopheakpanhaportfolio.netlify.app/materials/swerve-drive-hero.png" alt="Swerve-drive robot" style="width: 100%; border-radius: 8px;" loading="lazy">
<img src="https://dinsopheakpanhaportfolio.netlify.app/materials/swerve-architecture.png" alt="System architecture" style="width: 100%; border-radius: 8px;" loading="lazy">
</div>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: var(--space-4); margin-top: var(--space-4);">
<iframe src="https://www.youtube-nocookie.com/embed/0R4cwXsbjWk" title="Lookahead-based path tracking" style="width: 100%; aspect-ratio: 16 / 9; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
<iframe src="https://www.youtube-nocookie.com/embed/9ClcoE87dZw" title="Swerve-drive robot path tracking" style="width: 100%; max-width: 315px; aspect-ratio: 9 / 16; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
</div>
</div>

<div class="section-card" markdown="0">
<h3>Autonomous Indoor Food Delivery Robot (Thesis)</h3>
<p class="text-muted">DCLab, Institute of Technology of Cambodia · 2025 to 2026 · ROS 2 Humble, Nav2, SLAM Toolbox, AMCL, Jetson Orin Nano, RealSense D435</p>
<p>Together with a teammate, I built a differential-drive delivery robot from scratch, including the electrical system and a CANopen motor drive stack, and set up Nav2 so the robot maps a classroom, localizes, drives to a goal and replans around obstacles that were not in the map. A keepout mask stops the planner from routing under tables, and a depth camera detects obstacles added after mapping.</p>
<ul>
<li>10 of 10 trials reached the goal with zero collisions.</li>
<li>Mean physical position error of 0.256 m.</li>
</ul>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: var(--space-4); margin-top: var(--space-4);">
<img src="https://dinsopheakpanhaportfolio.netlify.app/materials/indoor-delivery-hero.jpg" alt="Indoor delivery robot" style="width: 100%; border-radius: 8px;" loading="lazy">
</div>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: var(--space-4); margin-top: var(--space-4);">
<iframe src="https://www.youtube-nocookie.com/embed/36Xstqjolxg" title="Autonomous food delivery robot" style="width: 100%; aspect-ratio: 16 / 9; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
<iframe src="https://www.youtube-nocookie.com/embed/7Au0h4lYpns" title="Autonomous food delivery robot" style="width: 100%; aspect-ratio: 16 / 9; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
<iframe src="https://www.youtube-nocookie.com/embed/6is34BcX-9I" title="Autonomous food delivery robot simulation" style="width: 100%; aspect-ratio: 16 / 9; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
<iframe src="https://www.youtube-nocookie.com/embed/mZaEWtkU5vU" title="Autonomous food delivery robot" style="width: 100%; max-width: 315px; aspect-ratio: 9 / 16; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
<iframe src="https://www.youtube-nocookie.com/embed/RdwP9cqwr-o" title="Autonomous food delivery robot navigation" style="width: 100%; max-width: 315px; aspect-ratio: 9 / 16; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
</div>
</div>

## Robot Arms

<div class="section-card" markdown="0">
<h3>Face Tracking Teleoperation with SO-ARM101</h3>
<p class="text-muted">Exchange semester, France · 2025 · Python, OpenCV, dlib</p>
<p>Normal teleoperation of the SO-ARM101 needs a second leader arm moved by hand. I led this project as Scrum Master and built a hands-free system where a single webcam and dlib facial landmarks control the arm: head yaw moves the base, head pitch moves the wrist, and mouth opening controls the gripper, at 60 Hz.</p>
<ul>
<li>A deadband removes the ±2.0 jitter in raw head yaw and pitch, so the arm stays still when the head is still.</li>
</ul>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: var(--space-4); margin-top: var(--space-4);">
<iframe src="https://www.youtube-nocookie.com/embed/ULV6JxhXbB4" title="Face tracking teleoperation with SO-ARM101" style="width: 100%; max-width: 315px; aspect-ratio: 9 / 16; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
</div>
</div>

## Industrial Automation

<div class="section-card" markdown="0">
<h3>Pick-and-Place with an ABB Robot Arm</h3>
<p class="text-muted">ABB industrial robot</p>
<p>A programmed pick-and-place routine running on an ABB industrial robot arm.</p>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: var(--space-4); margin-top: var(--space-4);">
<iframe src="https://www.youtube-nocookie.com/embed/8rvLOJjhovw" title="Industrial ABB robot arm pick-and-place" style="width: 100%; aspect-ratio: 16 / 9; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
</div>
</div>

<div class="section-card" markdown="0">
<h3>Conveyor Sorting System with PLC and HMI</h3>
<p class="text-muted">PLC, HMI</p>
<p>A conveyor sorting system controlled by a PLC and operated from an HMI panel.</p>
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: var(--space-4); margin-top: var(--space-4);">
<iframe src="https://www.youtube-nocookie.com/embed/rQ5fnVoLUaU" title="Conveyor sorting system with PLC and HMI" style="width: 100%; aspect-ratio: 16 / 9; border: 0; border-radius: 8px;" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen loading="lazy"></iframe>
</div>
</div>
