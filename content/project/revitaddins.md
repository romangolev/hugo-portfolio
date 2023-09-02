---
title: "Revit Add-ins development"
description: "Bundle of tools and enhancements for Revit"
#repo: "#" # delete this line if you want a blog-like page
tags: ["Revit", "C#"]
weight: 2
draft: false
---

### C#(.NET) Revit add-ins
Revit as an windows application uses .NET libraries and supports application written in C#, Python or VBNet. The code should be compiled into .dll file or set of files and then placed into one from supported directories. Basically C# Add-ins tend to exceute commands much faster within Revit environment and usually proves to be much stable due to the the fact that they does have less dependiences. 
The other thing that is very important is the possibility to implement much complex scenarious to interract with Revit. There is a great opportunity to build an app within an app to facilitate the automation needs and cover the mostly all demands of the design pipeline. Nonetheless the power of the automation development is limited by RevitAPI and sometimes it's possible to stumble across the API limitations. 
There are a lot of solutions for Autodesk Revit on the market like [DiRoots](https://diroots.com/), [BimOne](https://bimone.com/en/apps-and-scripts/) and a lot of integration plugins for another software, like bridges to Grasshopper or Tekla, integrations with ERP systems, rendering engines like VRay and Lumion. 

On my own I have also developed [RG Tools](https://github.com/romangolev/RG-Tools) Add-in in order to ease the process of BIM Coordination and help BIM Engineers organize the model. It has similar features that [pyArchitect](https://github.com/romangolev/pyArchitect) extension has, but does not require any other Add-in to be installed beforehand. 

Check this out, it goes under the GNU General Public License v3.0 and free for use! Unfortunally since it's an open-source application and lacks funding it's not signed by the certificate and would prompt a user approval every time it starts. 

---