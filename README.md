# PanaromaAnalysis


### Input : Video 

### 1. Removing foreground objects
#### Run `ForegroundExtraction.ipynb`
- Input needed : video with foreground object moving
- Detects and extracts person
- Saves extracted foreground frames in a new folder
- Fills remaining background holes 
- Saves extracted background frames in a new folder


### 2. Create Panorama with background
#### Run `PanoramaCreation.ipynb`
- Input needed : background video only
- Selects key frames from background video and saves it in new folder
- Creates panorama using selected frames
