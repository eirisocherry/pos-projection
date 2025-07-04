# Position Projection
An After Effects tool that allows you to quickly extract 3d coordinates and place any object to it  
Requirement: Position pass and Camera (or Depth pass and Camera)

## Installation
1. Download the tool: https://github.com/eirisocherry/pos-projection/releases  
2. Move the `Pos Projection` folder and `Pos_Projection.jsx` script to:  
`C:\Program Files\Adobe\Adobe After Effects <version>\Support Files\Scripts\ScriptUI Panels`  
3. Restart After Effects.  



## Usage

<details>
<summary> Setup </summary>
<br>

1. Open After Effects  
2. Go to `Window`, scroll down and open `Pos_Projection.jsx`  
3. The script panel will open, it's dockable  
4. Import 3d camera data  
CSGO: https://www.youtube.com/watch?v=78Y_Y-i5h2c  
COD4: https://www.youtube.com/watch?v=ZKsAgvfdi4I&list=PLiyMyFJsq2_VeOvBGMmrXcSAouRKO_hUB  
5. Import a depth map  
6. Select the depth map and setup a projection by pressing **[+]** button  
7. Adjust **'Depth settings':**  

**'Black is Near'** check it if a black color is near on your depth map, uncheck if it's not.  

**'Far'** the farthest depth point value:  
a) If the depth is normalized to [0..1] rgb range, then set far to:
CSGO (if you use my cfgs): regular `4096`, exr: `25000`  
CS2 (if you use my cfgs): regular `4096`, exr: `25000`  
COD4: `4080`  

b) If your depth is not normalized (rgb values are higher than), then set `Far` to `1`  
8.  Project any objects you want.  

- The script is heavy and may crash your After Effects, but don't worry!  
It automatically saves your project before doing any actions, so even if your AE will crash, you will not lose any of your progress  
- 'Auto Orient' works only with EXR depth maps  

<br>
</details>



<details>
<summary> Spot Light Matte </summary>
<br>

<br>
</details>



<details>
<summary> Rect Light Matte </summary>
<br>

<br>
</details>


<details>
<summary> Keyframes </summary>
<br>

When you project 'Keyframes', they are being stored in the 'Collected Keyframes' group  

<br>
</details>



<details>
<summary> Solid </summary>
<br>

When you project a 'Solid', it takes properties from 'Projected Solid' and color from 'Projection settings'  
`Ctrl + Shift + Y` to open 'Solid' settings  

<br>
</details>



<details>
<summary> 3D+2D null </summary>
<br>

<br>
</details>



<details>
<summary> Link-Bake </summary>
<br>

If you want to adjust position & orientation of an object:  
1. Press [⚙] button.  
2. Select 'Depth for Projection' and layers you want to make controllers for.  
3. Press [Link] button and adjust positions.  
4. To apply changes, select controllers and press [Bake] button.  

https://github.com/eirisocherry/3d-point-depth-projection/assets/115040224/50e2767d-9676-4130-8c9f-919d189ae79b  

<br>
</details>



## Credits
https://www.youtube.com/@shy_rikki  
