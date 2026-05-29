---
sidebar_position: 1
---

# Points Manager Setup (Inspect Points Manager)

---

## Overview

> If you will click on little arrow on side of **Examine Manager** you will see many objects, look at object named <span style={{color: '#ff8011'}}>**InspectPoints Manager**</span> and when you will click on <span style={{color: '#ff8011'}}>**InspectPoints Manager**</span>, you will see a script named <span style={{color: '#ff8011'}}>**Points Manager**</span>.

---

## Setup

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\50.png)
</div>
<br />

### Reference

- **ExamineManager** → Add your examineManager reference here.

### General Settings

- **InspectPanel** :-

> It is just a background on which the information about the inspect point will show.

> Here you have to add your **inspect panel** that you will find under **ExamineManager UI** there will be a object named as <span style={{color: '#ff8011'}}>**Inspect Panel - PivotPoint**</span> just drag and drop that in **InspectPanel** field.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\51.png)
</div>
<br />

- **InspectInfoText** :- 

> It is the text that will show the information of inspect point.

> You will find it under **Inspect Panel - PivotPoint** there will be a object named **Visual** under that you will find <span style={{color: '#ff8011'}}>**InspectInfo**</span> just drag and drop it in your **InspectInfoText** field.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\52.png)
</div>
<br />

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/2026-05-09 12-12-48-71.mp4" type="video/mp4" />
  </video>
</div>
<br />

- **FollowInspectPoint** → Enable it, if you want your **Inspect Panel** to follow your **InspectPoint** and when disabled **Inspect Panel** will stay on one position.

<div style={{textAlign: 'center'}}>
  <video controls width="80%">
    <source src="/Arc-ExamineSystemDoc/Videos/video14.mp4" type="video/mp4" />
  </video>
</div>
<br />

After that you will see two properties under **FollowInspectPoint**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\53.png)
</div>
<br />

- **HorizontalGap** → Here you can adjust horizontal gap between **Inspect Point** and **Inspect Panel**.
- **VerticalGap** → Here you can adjust Vertical gap between **Inspect Point** and **Inspect Panel**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\54.png)
</div>
<br />

---

### Inspect Panel - PivotPoint UI Explained

Now we can talk about **Inspect Panel - PivotPoint Setup** and about its childrens.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\51.png)
</div>
<br />

- **Inspect Panel - PivotPoint** → It is just a parent holding the **Visual** and **InspectInfo**.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\55.png)
</div>
<br />

- **Visual** → It is the background on top of which the information about that inspect point will show

→ You can change it if you want as it is just a simple **Image** component.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\56.png)
</div>
<br />

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\57.png)
</div>
<br />

- **InspectInfo** → It is the **Text** component that will show the information about the inspect point.

<br />
<div style={{textAlign: 'center'}}>
![Alt text](\img\58.png)
</div>
<br />

<span style={{fontSize: '22px'}}>**Done...🎊**</span>
