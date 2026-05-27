---
sidebar_position: 2
---

# 🎥 Camera setup

---

## Overview

In this examine system you can use your **Main Player Camera** as examine view or you can use a **Dedicated Camera** as examine view.

---

In your **Prefabs** folder you will find a object named <span style={{color: '#ff8011'}}>**ExamineCameraOverlay**</span>.


![Alt text](\img\14.png)

<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>The highlighted prefab</p>

Drag <span style={{color: '#ff8011'}}>**ExamineCameraOverlay**</span> under your **Player Camera** or under your **Dedicated Examine Camera** as child.

:::danger[Must Do!!]

Reset your <span style={{color: '#ff8011'}}>**ExamineCameraOverlay**</span> **Rotation** and **Position**.

:::

<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\video32.mp4" type="video/mp4" />
  </video>
</div>

Must Watch!!

<br />

:::danger[Important]

In <span style={{color: '#ff8011'}}>**ExamineCameraOverlay**</span> under rendering in culling mask only choose **Examinable** layer and disable other.

<div style={{textAlign: 'center'}}>
![Alt text](\img\33.png)
</div>

:::

---

<span style={{fontSize: '20px'}}> **Now in ExamineManager** </span>

#

Look for field named **OverlayCamera** in **ExamineManager**.

<div style={{textAlign: 'center'}}>
![Alt text](\img\6.png)
</div>

Now just drag and drop your ExamineCameraOverlay.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\2026-05-01 11-01-58-52.mp4" type="video/mp4" />
  </video>
</div>

---

> This is how you can add a background behind → [Background Setup](BackgroundSetup.md)