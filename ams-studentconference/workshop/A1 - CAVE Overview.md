# Appendix 1: Workshop CAVE Demonstration

## Plot multiple datasets on one map (time matching) + add maps/configure

### `Surface → 60 min RAWS Plot` (menu bar)

Increase Magnification - `Mag: 1.5` (dropdown in toolbar)

Use arrow keys or buttons to go forward/back in time

Notice the frame count

Time valid for +/-30 min at top of the hour

### `Satellite → GOES East CONUS → 0.64 um Red Visible Band` (menu bar)

Notice the bottom right `Creating Image Tiles` - loading

Use arrow keys to go back in time - notice satellite updating only every 60 min

GOES updates every 5 minutes - time matching is important!

### Resource Stack (bottom right - right click in map to cycle through)

#### Product View

Right click and hold on the GOES 19 product - select `Time Match Basis` from the pop-up menu - should move to GOES-19 product

Use arrow keys and notice satellite updates every 5 minutes

#### Simple View 

Current date/time that product is valid for

#### Map View

Map name

### Load Maps

#### Maps → CWA’s (menu bar)

Right click and hold on `County Warning Area`  - select `Change color → Yellow` (Resource Stack - map view)

Right click and hold on `County Warning Area`  - select `Line width → 2 pixels` (Resource Stack - map view)

#### Maps → Interstates (menu bar)

Toggle on/off - Left Click on `Interstates` (Resource Stack - map view)

Unload Product - Right click and hold on “Interstates” - select “Unload” (Resource Stack - map view)

## multi-dataset exploration + interface to parallel sampling + saving procedure

New Map: `File → New Map` (Menu bar)

Unload CWA: `Clear` (Toolbar) 

### Load 4 panel products

Right click and hold, select `Change Panel Layout → 4 Panel Layout`

Zoom in/out (mouse scroll) - applies to all panels

### Load to top left panel

Right click and hold in top left map panel - select `Load to this panel`

Load Model Data: `Models → HRRR → Sfc Temperature and Wind`

### Load to top right panel

Right click and hold in top left map panel - select `Load to this panel`

Load Model Data: `Models → GFS20 → Sfc Temperature and Wind`

### Load to bottom right panel

Right click and hold in top left map panel - select `Load to this panel`

Load Model Data: `Models → NAM12 → Sfc Temperature and Wind`

### Load to bottom left panel

Right click and hold in top left map panel - select `Load to this panel`

Load Model Data: `Models → RAP13 → Sfc Temperature and Wind`

### Resource Stack
`[Model] [Product] [Current day of month] [Model Run Hour] [Forecast Hour] [Valid Forecast Time]`
`[HRRR] [Sfc Temperature Img (F)] [15] [22] [17HR] [Fri 15:00Z 16-Jan-26]`

Turn on Sampling: Right click and hold in any of the map panels - select `Sampling`

Rename Tab: Right click and hold on tab - select `Rename Tab` - 

Name tab `Sfc Model 4 Panel` - click `OK` (GUI)

Save procedure: `File → Procedures → New Procedure` (menu bar)

Copy In (GUI)

Save: as `tiffanys_procedures` - `OK` - `close` (GUI)

`Clear` (toolbar)

Open procedure: `File → Procedures → Open Procedure` (menu bar)

Open `tiffanys_procedures` - `OK` (GUI)

Select `Sfc Model 4 Panel` - `Load` (GUI)

## Default 4 panel radar data + cycling through panels
`Koax → All Tilts Base Data` (data menu)

Change number of frames: `Frames - 30 (toolbar)

Up and Down arrow keys - cycle through tilts (keeps the same time/scan)

Front and Back arrow keys - cycle through time (keeps the same tilt angle)

Use Period Key on NumPad to toggle between products

To blow up a single panel, but keep all data accessible - click the Del key - keep pressing it will rotate through all 8 products

Press ”delete” key - zooms into top left panel

Continue to press ”delete” key - cycles through each of the 8 products in zoomed in mode

Press “end” key to get back to 4 panel layout

## Screen real estate + CAVE calculations and derivations

Show side panes: `View → 5 Pane Layout` (menu bar)

Swap panes from main to side: Right click in side pane

Load Split Snow: `Satellite → GOES -East CONUS → Channel Differences → Split Snow (1.61 - 0.64um)`

**CAVE is doing this calculation**

Change scales: “CONUS” → “GOES East Full Disk” (toolbar)

## Show and edit soundings

`Upper Air → US Central → Oklahoma City (KOUN)` (menu bar)

Drag “NSHARP bar to bottom”

Zoom, toggle through times

Select `EditGraph` button

Adjust points in sounding by dragging them - see how calculations are updated

`Reset` button to go back to default sounding

## Find data not in menus

Look at other model data: `Models → Volume Browser` (menu bar)

Sources: `Volume → GFS20` (products with a green box are available data)

Fields: `Stability → Lapse Rates`

Planes: `Pres → 1000MB-700MB`

Load (loads as a contour)

Change to an image: Right click and hold on GFS Product in resource stack → `Load as image`

Product Browser: `CAVE → Data Browsers → Product Browser` (menu bar)

Grid and Satellite data - similar hierarchy as to how to query in python
