[![Made with Unity](https://img.shields.io/badge/Made%20with-Unity-57b9d3.svg?style=flat&logo=unity)](https://unity3d.com)
[![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php)
[![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://github.com/dennishnf/project-xr-glasses/issues)
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
     
[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Download%20and%20use%20the%20Project%20XR%20Glasses&url=https://github.com/dennishnf/project-xr-glasses&hashtags=unity,augmentedreality,unity3d,facedetection,arkit)


# Project XR Glasses


## Description

This project consists of the development of an augmented reality application that allows users to quickly and easily try on various models of glasses and visualize in real time the price as well as their design. 


## Unity version

Unity Version: 2020.3.20f1   
Developing Platforms: Ubuntu 20.04 LTS and Windows 10    
Intended Devices: >= Android 8.1.0 Oreo   
Packages: AR Fundation, AR Core XR Plugin, ARKit Face Tracking, ARKit XR Pluigin   


## Flowchart

<p align="center">
<img src="imgs_/diagram.png" alt="Flowchart" width="350"/>
</p>


## Pseudo code: 

```
start the face detection
perform landmark extraction
run pre defined glasses models

for selected_glasses in models_list:
	anchor the points of face with glass 3d model
	show the face with the glasses
	read option of glasses
```


## Updates

### Update 23 Nov 2021:

Face detection and extraction of the most relevant points of the face were successfully implemented. The AR Foundation and ARKit Face Tracking packages were used for this purpose. The main challenges faced were: compatibility with android devices and successfully configuring the building options. 

<p align="center">
<img src="imgs_/face-mask.png" alt="Examples" width="600"/>
</p>


### Update 30 Nov 2021:

Different lens models were collected in .obj format, but were converted to .prefab by creating a prefab object and then pulling the .obj lenses into that object. 

<p align="center">
<img src="imgs_/glasses.png" alt="Examples" width="600"/>
</p>


### Update 07 Dec 2021:

Successfully performed the attachment of a reference point of the face, and the placement of the lenses. This was done in several stages, in the first tests a prefab object was instantiated, then the position of the eyes was extracted and the position and rotation transformations were instantiated to that prefab object.

<p align="center">
<img src="imgs_/glasses-face.png" alt="Examples" width="600"/>
</p>



## Using this repository

Download or clone, then Settings Build and Run, then Switch Platform to Android.

Also, install the packages: AR Fundation, AR Core XR Plugin, ARKit Face Tracking, ARKit XR Pluigin.    



## References

- [Setting Up AR Foundation](https://learn.unity.com/tutorial/setting-up-ar-foundation#5fe2be51edbc2a1f5e69872f)    
- [ARKit Face Tracking](https://docs.unity3d.com/Packages/com.unity.xr.arkit-face-tracking@4.1/manual/index.html)    
- [Unity AR Foundation Tutorial - Getting Started with Face Tracking](https://www.youtube.com/watch?v=y0L_AdJICEU)    
- [Unity3d ARKit Face Tracking and placing face game objects with anchor data
](https://www.youtube.com/watch?v=JQEovMKq2U0)    



## Group

- Miky ([@MrMazagngy](https://github.com/MrMazagngy))   
- Yao ([@iyfyao](https://github.com/iyfyao))    
- Dennis ([@dennishnf](https://github.com/dennishnf))   




<!---

git pull
git add -A
git commit -m "v0"
git push -u origin main

--->

