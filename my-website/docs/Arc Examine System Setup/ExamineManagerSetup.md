---
sidebar_position: 3
---
# 📟 Examine Manager setup

> <span style={{color: '#888888'}}> How you can setup your Examine Manager </span>

---

## Overview

when you will first open **Examine Manager** you will see this.
<br />
<div style={{textAlign: 'center'}}> 
  <img src="/Arc-ExamineSystemDoc/img/10.png" alt="Alt text" style={{ width: '300px', height: 'auto' }} /> 
</div>
<br />
---
## Explaining

### References

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\11.png)
</div>
<br />

- **RayOrigin** → In this field you have to add your **GameObject** like **Player Camera** that will be the starting point of your raycast.

### Camera Settings

Here you will find two fields.

-- **Camera Type** and **Overlay Camera**

- **Camera Type**:-

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\12.png)
</div>
<br />

Here you can choose to use **MainCamera** or **Dedicated ExamineCamera**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\13.png)
</div>
<br />

If you will select **MainCamera** it will automatically detect the camera and use it as examine view.

:::note

Ensure that **MainCamera** have tag <span style={{color: '#ff8011'}}>**MainCamera**</span>.

:::

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\15.png)
</div>
<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>View with main player camera</p>
<br />

And now if you will select **Different Camera** you will see two other options.

-- **SeparateCamera** and **MainCamera State**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\16.png)
</div>
<br />

- **SeparateCamera**

In this field you have to drag your separate examine camera. 

- It will be used as your examine view, this can be useful if you want to use different camera rather than your main camera.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/2026-05-03 11-33-36-72.mp4" type="video/mp4" />
  </video>
</div>

:::note

Remember to hide **Examine Camera**, it will be automatically enabled when needed.

:::

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\17.png)
</div>
<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>View with different examine camera</p>
<br />

- **MainCamera State**

Here you can choose what happens to main camera as we will switch to different examine camera in examine state there are two options to select.

-- **None** and **Hide**
<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\18.png)
</div>
<br />

| Options | Description |
|---------|-------------|
| **None** | Nothing will happen.|
| **Hide** | Main camera will get hidden when you will enter examine state and again show when you will exit examine state.|

---

- **OverlayCamera**

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\19.png)
</div>
<br />

You have to drag your **ExamineOverlayCamera** here.

Look at <span style={{color: '#ff8011'}}>**Camera Setup**</span> page for all other details about OverlayCamera → 
[Camera Setup](CameraSetup.md).

### Properties

Here you will see three fields.

- **RayLength**, **DistanceFromCamera** and **Placement Type**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\20.png)
</div>
<br />

- **RayLength** → It is length of the raycast that lets you interact with examinables.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/2026-05-03 13-45-55-00.mp4" type="video/mp4" />
  </video>
</div>

- **DistanceFromCamera** → It defines at what distance your examinable will be placed on screen when you will enter the examine state.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/video2.mp4" type="video/mp4" />
  </video>
</div>
<br />

- **Placement Type**

Here you can choose between **Centre** and **Custom**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\21.png)
</div>
<br />

- **Centre** → If you choose will centre than your examinable will be placed in centre on screen by default.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\15.png)
</div>
<br />

- **Custom**:-

Here you can choose custom position on screen to place your examinable.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\22.png)
</div>
<br />

Here are two fields you can change.

- **Placement X** → Defines position in X axis.
- **Placement Y** → Defines position in Y axis.

Default value is set to **Centre**, change values to change your examinable position on screen.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\23.png)
</div>
<br />

### Sounds

Here you will see one option.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\24.png)
</div>
<br />

- **Have Sounds** → Enable it if you want to have sounds in your examinables.

After enabling you will see another option.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\25.png)
</div>
<br />

In this field you have to add your <span style={{color: '#ff8011'}}>**AudioSource**</span> from where the sounds will play.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/2026-05-08 19-23-16-79.mp4" type="video/mp4" />
  </video>
</div>
<br />

### Events

Here you will find two fields.

- **OnExamineStart** and **OnExamineEnd**

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\26.png)
</div>
<br />

- **OnExamineStart** → Here you can add a **Custom Events** that will play when you will enter examine state.
- **OnExamineEnd** → Here you can add a **Custom Events** that will play when you will exit examine state.


---

And that the end you will see one option named **Visualize Ray** → Enable it, if you want to visualize your raycast in real-time.

<span style={{fontSize: '22px'}}>**Done..🎊**</span>