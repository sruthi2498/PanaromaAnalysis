# PanaromaAnalysis


### Input : Video 


https://user-images.githubusercontent.com/22856887/207781703-203e5d95-a2ce-42e5-9c67-d20a495727b9.mov


### 1. Removing foreground objects
#### Run `ForegroundExtraction.ipynb`
- Input needed : video with foreground object moving
- Detects and extracts person
- Saves extracted foreground frames in a new folder
<img src="https://user-images.githubusercontent.com/22856887/207782454-95b37b5d-b7e5-4559-8644-ba4e34a69864.png" width="500" >
- Fills remaining background holes 
- Saves extracted background frames in a new folder 
- <img src="https://user-images.githubusercontent.com/22856887/207783470-c4af1330-843f-403b-ace0-c540fbfaa71e.png" width="500" >
- Creates background and foreground videos

https://user-images.githubusercontent.com/22856887/207783385-bdaf41f2-0d3d-4ae7-b723-9c99c8d9d596.mov


https://user-images.githubusercontent.com/22856887/207783592-ee9602cd-80f3-4a8b-a397-234c30e3c32d.mov



### 2. Create Panorama with background
#### Run `PanoramaCreation.ipynb`
- Input needed : background video only
- Selects key frames from background video and saves it in new folder
- Creates panorama using selected frames
<img src="https://user-images.githubusercontent.com/22856887/207783765-27d6822e-52f1-4044-b5f7-8fc843f9d19d.png" width="500" >

### 3. Motion Trails on Panorama
#### Run `MotionTrails.ipynb`
- Input needed : foreground frames, background frames and background panorama
- Selects background frames that have good number of matching keybpoints with panorama
- Selects corresponding foreground frame and warps it to paste it on the panorama
![motion-trails](https://user-images.githubusercontent.com/22856887/207785095-299b74ba-7ef7-485c-919e-5997d7358d27.png)

