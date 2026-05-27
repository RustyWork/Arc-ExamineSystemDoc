---
sidebar_position: 1
---
# ⚱ Examinable Setup

> <span style={{color: '#888888'}}>After all that we can move to finally creating the examinable</span>

#

Now you add **Examinable** script in examine object.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video5.mp4" type="video/mp4" />
  </video>
</div>
<br />

After adding the **Examinable** in object you will see this.

<br />
<div style={{display: 'flex', gap: '10px'}}>
  <img src="/img/34.png" alt="Image 1" width="50%" />
  <img src="/img/35.png" alt="Image 2" width="50%" />
</div>
<br />

#### It may look like there are lots of options but it is fairly easy to setup.

---

## Setup

### General

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\36.png)
</div>
<br />

- **ItemName** → Here you can add here your examinable object name, it will be displayed on **UI**.
- **Description** → add your description about your examinable object here, it will be displayed on **UI**.

:::tip[Learn More!!]
**UI** explained → [UI Setup](@site/docs/Arc%20Examine%20System%20Setup/UISetup.md).
:::

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\37.png)
</div>
<br />

- **ItemCanMove** → Enable it, if your examinable can be moved in run-time, it will capture its new moved position and use it later to place
that examinable on its new position when exit examine state. 

Note - it only captures examinable position while we are not in examine state.

- **HaveChildren** → Enable it, if you have children under your examinable object, after enabling you will see this.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\38.png)
</div>
<br />

And if you're feeling lazy today and don't wanna add children's manually just click on **Detect children's** it will add them automatically.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video7.mp4" type="video/mp4" />
  </video>
</div>
<br />

### Rotation Settings

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\39.png)
</div>
<br />

- **RotateSpeed** → This float controls at what speed your examinable object will rotate.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video8.mp4" type="video/mp4" />
  </video>
</div>
<br />

- **SeparateAxis** → Enable it, if you want different speed for **X** & **Y** axis. after enabling it you will see this.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\40.png)
</div>
<br />

Here you can edit your X & Y speed individual.

### Zoom Settings

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\41.png)
</div>
<br />

- **DefaultSize** → Here you can add your default size that you want every time you start your examine state.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video9.mp4" type="video/mp4" />
  </video>
</div>
<br />

- **CanWeZoom In & Out** → Enable it, if you want to zoom In & Out in your examinable object. After enabling you will see this.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\42.png)
</div>
<br />

- **ZoomSpeed** → here you can control your zoom in & out speed.
- **ZoomMinRange** → here you can set your minimum zoom range of your examinable object.
- **ZoomMaxRange** → here you can set your maximum zoom range of your examinable object.
- **ZoomSmoothing** → here you can set smoothing inbetween of your zoom. [Recommended value [5]]

### Inspect Points

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\43.png)
</div>
<br />

Here you can add your **Inspect Points** if you have them in your examinable object.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video10.mp4" type="video/mp4" />
  </video>
</div>
<br />

### HighLight Settings

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\44.png)
</div>
<br />

- **HighlightWhenHovered** → Enable it, if you want to show a emission highlight when player hovers over the examinable object. After 
enabling this will show.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\45.png)
</div>
<br />

- **EmissiveColor** → you can control your emissive color from here.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video11.mp4" type="video/mp4" />
  </video>
</div>
<br />

- **Intensity** → here you can control the intensity of your emissive color.

After that you will see a empty list of **Renderer Objects**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\46.png)
</div>
<br />

Here you can add your objects on which you want to show highlight.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video12.mp4" type="video/mp4" />
  </video>
</div>
<br />

### Sounds Settings

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\47.png)
</div>
<br />

- **Have Sounds** → Enable it, if you want sounds in this examinable object. After enabling you will see this.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\48.png)
</div>
<br />

- **Pick Sound** → here you can add your <span style={{color: '#ff8011'}}>**AudioClip**</span> sound of picking, this sound will play
when you will enter in examine state.
- **Drop Sound** → here you can add your <span style={{color: '#ff8011'}}>**AudioClip**</span> sound of dropping, this sound will play
when you will exit in examine state.
- **Volume** → here you can adjust your volume of sound.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="\Videos\Video13.mp4" type="video/mp4" />
  </video>
</div>
<br />

:::note

If you don't have sound for dropping you can leave the **Drop Sound** field empty and same for picking.

Ensure that **HaveSounds** is enabled in **ExamineManager**, All details about [Sounds Setup in ExamineManager](@site/docs/Arc%20Examine%20System%20Setup/ExamineManagerSetup.md), Find title named **Sounds**.

:::

### Events

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\49.png)
</div>
<br />

Here you can add your **Customs Events** .

- **OnExamineStart** → Plays on entering in examine state.
- **OnExamineEnd** → Plays on exiting of examine state.

---

:::important

Please make sure there is a **Collider** in the examinable object and that **collider** is not interfering with other **colliders** to make sure proper interaction. [Recommended adding a MeshCollider]

:::