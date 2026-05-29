---
sidebar_position: 7
---

# 🖼 Background Setup

> How you can setup your background behind your examinable objects.

---

## Setup

> Setting up background behind your examinable objects is fairly easy.

If you go under the **Prefabs** folder, you will find a folder named **Backgrounds**, and under that folder you will find two objects.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/99.png" alt="Background Prefabs" />
</div>

<br />

First prefab is for <span style={{color: '#ff8011'}}>**Blur Effect**</span> background and second is for <span style={{color: '#ff8011'}}>**Solid Background**</span>.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/100.png" alt="Blur and Solid Background" />
</div>

<br />

And to use the effect, just drag and drop your prefab under **ExamineCameraOverlay**.

---

## Blur Effect Setup

First add the **BlurCamera** under **ExamineCameraOverlay** as child.

<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/video28.mp4" type="video/mp4" />
  </video>
</div>

<br />

:::danger[Note]

- Please reset the blur camera position and rotation after adding blur camera under **ExamineCameraOverlay**.
- Ensure that <span style={{color: '#ff8011'}}>**BlurCamera**</span> layer is set to Examinable with its child objects.

:::

Now if you go inside the **BlurCamera** object, you will find a script named <span style={{color: '#ff8011'}}>**Blur Manager**</span>.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/7.png" alt="Blur Manager" />
</div>

<br />

- **Blur Camera** → Add your **Blur Camera** reference here.
- **Blur Material** → Explained below.

Drag your <span style={{color: '#ff8011'}}>**BlurMaterial**</span> into the **Blur Material** field.  
You will find <span style={{color: '#ff8011'}}>**BlurMaterial**</span> under the **Arc Examine System** folder → **Shaders** folder → **UI Blur** folder.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/8.png" alt="Blur Material" />
</div>

<p style={{color: '#888888', marginTop: '-1rem', textAlign: 'center'}}>
The highlighted Material
</p>

<br />

Now drag <span style={{color: '#ff8011'}}>**BlurMaterial**</span> into the **Blur Material** field.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/7.png" alt="Blur Material Field" />
</div>

<br />

And now, under **BlurCamera**, you will find <span style={{color: '#ff8011'}}>**BlurCanvas**</span>.  
In that **BlurCanvas**, there is a field named **Render Camera**, and ensure **ExamineCameraOverlay** is added in the render camera field.

<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/video29.mp4" type="video/mp4" />
  </video>
</div>

<br />

## <span style={{fontSize: '22px'}}>Blur-Background Object Explained</span>

<div style={{margin: '25px 0'}} />

> Under the **BlurCanvas** you will find an object named <span style={{color: '#ff8011'}}>**Blur-Background**</span>. It will display your blur effect.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/106.png" alt="Blur Background" />
</div>

<br />

- **Blur-Background** → It is a simple **UI Image** component, which will display the blur effect.

:::caution[Important Note]

<p style={{color: '#ffffff', fontSize: '13px'}}>
⚠ Changing the <strong>Blur-Background</strong> size is not recommended.
</p>

:::

And in **Blur-Background** component we have to set the **Material** field to **BlurMaterial**.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/101.png" alt="Blur Background Material" />
</div>

<br />

You can adjust the **blur effect** blur strength and scale from its material.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/102.png" alt="Blur Settings" />
</div>

<br />

## <span style={{fontSize: '19px'}}>Result</span>

<div style={{margin: '25px 0'}} />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/video30.mp4" type="video/mp4" />
  </video>
</div>

<br />

---

## Solid Background Setup

> This is how you can add a solid background behind your examinable objects; it could be useful if you want a different style for your game.

Now to add it, add the <span style={{color: '#ff8011'}}>**Solid_BackgroundCanvas**</span> from your **Backgrounds** folder and add it as child of **ExamineCameraOverlay**.

And now, same as **BlurCanvas**, in <span style={{color: '#ff8011'}}>**Solid_BackgroundCanvas**</span> there is a field named **Render Camera**, and ensure **ExamineCameraOverlay** is added in the render camera field.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/104.png" alt="Solid Background Render Camera" />
</div>

<br />

## <span style={{fontSize: '22px'}}>Solid-background Object Explained</span>

<div style={{margin: '25px 0'}} />

Under <span style={{color: '#ff8011'}}>**Solid_BackgroundCanvas**</span> you will see an object named <span style={{color: '#ff8011'}}>**Solid-background**</span>.

<br />

<div style={{textAlign: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/105.png" alt="Solid Background Object" />
</div>

<br />

- **Solid-background** → It is a simple **UI Image** component, just set it to your background and done.

<br />

<div style={{display: 'flex', gap: '10px', alignItems: 'center'}}>
  <img src="/Arc-ExamineSystemDoc/img/103.png" alt="Background Image" width="50%" />
  <span style={{fontSize: '24px', flexShrink: 0}}>→</span>
  <img src="/Arc-ExamineSystemDoc/img/ExamineBackground.png" alt="Default Background" width="40%" />
</div>

<p style={{color: '#888888', marginTop: '0.5rem', textAlign: 'center', marginLeft: '50%'}}>
Default Background
</p>

<br />

## <span style={{fontSize: '19px'}}>Result</span>

<div style={{margin: '25px 0'}} />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/video31.mp4" type="video/mp4" />
  </video>
</div>

<br />

:::danger[Note]

Ensure that <span style={{color: '#ff8011'}}>**Solid_BackgroundCanvas**</span> layer is set to Examinable with its child objects.

:::

---

:::danger[Performance Tip]

Disable the **Examinable** layer under **Rendering** in **Culling Mask** from the player camera or from your dedicated examine camera  if you are using the **blur effect** or a **solid background**.

⚠ If you do not do this, it will impact performance.

:::