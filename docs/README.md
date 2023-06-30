<a name="ultitools"></a>
# UltiTools 🛠️

UltiTools is a powerful Blender add-on that enhances Blender's capabilities by providing various tools for modeling and asset creation. With UltiTools, you can expand Blender's functionality and improve your workflow. This documentation provides an overview of UltiTools and its features.

[![Video showcase](https://img.youtube.com/vi/I8yvBzNMHaM/0.jpg)](https://www.youtube.com/watch?v=I8yvBzNMHaM&ab_channel=Ultikynnys)

<a name="installation"></a>

## Installation 🚀

To install UltiTools, follow the steps below:

1. Download the add-on ZIP file from the [Blender Market](https://blendermarket.com/products/ultitools) ⬇️
2. Launch Blender and navigate to **Edit > Preferences** 
3. In the Preferences window, select the **Add-ons** tab 
4. Click the **Install** button 
5. Locate and select the downloaded ZIP file 
6. Click the **Install Add-on** button 
7. Enable the add-on by ticking the checkbox next to its name 
8. Configure any additional settings if required 
9. Click the **Save Preferences** button 

UltiTools is now installed and ready to use. 🎉

<a name="usage"></a>
## Usage 🧑‍💻

Once UltiTools is installed and enabled, you can access its features within Blender. For more additional information about each feature, refer to tooltips within Blender.

Here are some basic instructions for using the add-on:
1. Launch Blender and open your desired project 
2. Locate the UltiTools panel or menu in Blender's UI (found in the sidebar) 
3. Click on the add-on's options to activate specific features 
4. Adjust any parameters or settings as needed 
5. Interact with the objects or elements in your scene to apply UltiTools' functionality 



<a name="features"></a>
## Features ✨

UltiTools offers the following key features:

### Ulti Sage 🧙


Ulti Sage is the first tab you will see when you open UltiTools. It will show you relevant information according to what is selected and depending on what exists in the scene. <br>
![Ribbon view](./Sage.png)

### Smart Symmetrize 🔄
Perform actions that go beyond the capabilities of the Mirror Modifier. Mirror Shape Keys and bisect the mesh without mirroring the mesh itself.

[![Video showcase](https://img.youtube.com/vi/27xPZl3vi6c/0.jpg)](https://www.youtube.com/watch?v=27xPZl3vi6c&ab_channel=Ultikynnys)

### Mesh Data Merge 🧩
Easily combine Shape Keys or Vertex Groups.

[![Video showcase](https://img.youtube.com/vi/uetbQmzUdOk/0.jpg)](https://www.youtube.com/watch?v=uetbQmzUdOk&ab_channel=Ultikynnys)

### Quick Sculpt Mask 🎭
Save and load Sculpt masks using Vertex Groups, allowing for the application of selection as masks.

[![Video showcase](https://img.youtube.com/vi/A67Yu_MkNuQ/0.jpg)](https://www.youtube.com/watch?v=A67Yu_MkNuQ&ab_channel=Ultikynnys)

### Text Animation 📝🎬
Bring your Text Objects to life using keyframes and Python scripting.
Using python syntax you can define how the text objects behave. Here are some examples.
```python
hardcoded variables.
loc(object name) = location[3]
rot(object name) = angle[3]
scale(object name) = scale[3]
\n # newline
'' # Single quotes are used for string variables
"" # double quotes are used for text
```
Here is an advanced example from the included blend file. It may look complicated when the text script is in one line.
![Ribbon view](./Text.png)
With tabs it is much easier to understand how the text object will behave.
In this case it will inherit the properties of the object called "Location Test", which is the name of the text object in the screenshot.
```python
"Location\nX :" # static string
round(loc('Location Test')[0]) # x axis of object rounded to first digit

"\nY : " # static string
round(loc('Location Test')[1]) # y axis of object rounded to first digit

"\nZ : " # static string
round(loc('Location Test')[2]) # z axis of object rounded to first digit
```

[![Video showcase](https://img.youtube.com/vi/aNaJQEXH1FQ/0.jpg)](https://www.youtube.com/watch?v=aNaJQEXH1FQ&ab_channel=Ultikynnys)

### Sprite Sheet Gen 🎞️
Generate sprite sheets directly within Blender.

The tool generates a single image from an input folder filled with images.

It is ideal to set the render output folder as the Sprite Sheet input folder.
This way you can quickly turn your renders into sprites. Very useful when creating sprite sheets from blender simulations.

You can use the included example blend file to test this.

[![Video showcase](https://img.youtube.com/vi/BGtd6JSe1Ts/0.jpg)](https://www.youtube.com/watch?v=BGtd6JSe1Ts&ab_channel=Ultikynnys)

### Multi Camera Render 🎥🎥🎥
Render multiple cameras using unique frame ranges and output paths for each camera.

This tool works very well with **Sprite Sheet Gen 🎞️**

[![Video showcase](https://img.youtube.com/vi/SC3yCdjqBHI/0.jpg)](https://www.youtube.com/watch?v=SC3yCdjqBHI&ab_channel=Ultikynnys)

### Bonus Blend file 🎁
Includes a showcase of how Text Animation works. Same file as used in the video showcase.


## FAQ ❓
Here are some frequently asked questions about UltiTools

**Q:** I found a problem with the addon, what do I do?

**A:** Contact the author in [Contacts](#Conclusion-🎉) 

**Q:** How can I update UltiTools to a newer version? 

**A:** To update the add-on, download the latest version from the official website and follow the installation steps mentioned in the
[Installation](#Installation-🚀) section. 


## License 

UltiTools is licensed under the **Single User License**. This license grants you the following rights:

1. **Usage**: You are authorized to use UltiTools on a single device or computer. 

2. **Modifications**: You can modify UltiTools to suit your specific needs or preferences. 

3. **Personal Use**: You can use UltiTools for both non-commercial and commercial purposes. 

However, the Single User License imposes the following restrictions:

1. **Distribution**: You are not permitted to distribute or share UltiTools with others. 

<a name="conclusion"></a>
## Conclusion 🎉

Thank you for choosing UltiTools as your go-to Blender add-on. We hope that this documentation has provided you with a comprehensive understanding of UltiTools and its features. Remember to abide by the Single User License terms and conditions while utilizing the add-on. If you have any further questions or feedback, please feel free to contact me directly at Hussein.Ubeid@outlook.com. 📧

## Changelog 📋

### Version 0.4.3
- MultiCameraRender data now saved to camera data instead object to support object data linking.
- Ability to reverse Image order in SpriteSheetGenerate
- Added an button in [Object Mode] in the Select ribbon, which makes all objects selectable.
- Smart symmetrize edge clean up is more reliable.


### Version 0.4.2
- More hotfixes for 3.5 Blender support


### Version 0.4.1
- Hotfixed issues with smart symmetrize not doing anything.


### Version 0.4.0
- UI elements are now separated for each tool.
- Text animation overhauled 
- Improved performance and optimized resource usage. 
- Updated dependencies to the latest versions. 


