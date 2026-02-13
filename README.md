# PicSwipe

**A vibe-coded browser app to quickly review and sort large photo albums fully offline.**

Organize your photos with a swipe-style interface: keep, maybe, or discard images from your collection. Once you are done, it will generate a script that will sort the pictures into the right folders for easy manage.

**Important:** The app **cannot move or delete your files directly**—it only generates a script you can run manually to organize your images.

----------

## Features
-  **Fully offline**: no server processing, no need to deploy anything, just serve a simple index.html file

-   **Vibe-coded AI style interface**: lightweight, fast, and responsive.
    
-   **Swipe-style decisions**: keep, maybe, or discard images.
    
-   **Thumbnail overview**: see all your images at a glance.
    
-   **Undo support**: easily revert a previous decision.

-   **Script generation**: generates a platform-specific script (`.bat` for Windows, `.sh` for macOS/Linux) to move files into `keep`, `maybe`, and `discard` folders.
    
-   **Works in major browsers**: latest versions of Chrome, Edge, Firefox, and Safari.

## Deployment

The app must be served over **localhost or HTTPS** due to browser security restrictions for file access.

**Easiest way to run it locally:**

`python -m http.server 8000` 

Then open your browser and navigate to `http://localhost:8000`.

----------

## Usage

1.  Click **Open Folder** and select the folder containing your photos. Only `.jpg` and `.jpeg` files are supported.
    
2.  Use the buttons or keyboard shortcuts to decide for each image:
    
    -   `A` → Keep
        
    -   `W` → Maybe
        
    -   `D` → Discard
        
    -   `S` → Undo last decision
        
    -   `Arrow Left/Right` → Navigate between images
        
    -   `Z` → Toggle zoom
        
3.  After sorting, click **Finish & Get Script** to download a script that will move your images into `keep`, `maybe`, and `discard` folders.
    
4.  Run the script in the folder with your photos to reorganize them automatically.
    

----------

## Notes
    
-   Always make sure to **backup your photos** before running the script.
    

----------

## License

This project is **vibe-coded** and released under the **AGPLv3** license. Attribution and share-alike required.
