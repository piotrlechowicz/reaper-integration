### Integrating Korg nanoKontrol2 with reaper

1. Download reaper csurf integrator from 
https://stash.reaper.fm/v/38349/CSI%20beta.zip

the documentation is available here:
https://github.com/GeoffAWaddington/reaper_csurf_integrator/wiki	

2. Go to reaper resource path (sth like, `C:\Users\piotr\AppData\Roaming\REAPER`)
You can find resource path by going into reaper's action list and searching for 'Show REAPER resource path' 
(further denoted as ${reaper_resource})

3. From the downloaded file
	1. Put the `CSI` folder in Reaper resource path.
	1. Put `reaper_csurf_integrator.dll` in the UserPlugins folder in Reaper resource path

4. Copy the following files from this repository to the following locations in Reaper resource paths.  
	1. Instead of step between 9 and 13 in instruction
	copy `CSI-nano-korg-2/CSI.ini` file to `${reaper_resource}/CSI/`. Edit file, and change two numbers after the 
	name - it corresponds to the id of connected midi in and out device in reaper
	2. Copy files in folders `CSI-nano-korg-2/Surfaces` and `CSI-nano-korg-2/Zones` to `CSI` folder.
	
5. Open Korg Kontrol Editor and load `nano-korg-2-config/configuration_for_CSI.nktrl2_data` settings to 
your nanoKontorl2 device.