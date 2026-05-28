# Bavaria COP 1809
### Common Operating Picture — Flight of the Eagle Wargame
**U.S. Army War College — Napoleonic Studies**

---

## What This Is

A browser-based Common Operating Picture (COP) for the **Flight of the Eagle** 1809 Danube Campaign wargame. Built for use at the U.S. Army War College to track unit positions, issue move orders, calculate ETAs, and monitor contact between French and Austrian forces across the Bavaria theater of operations.

The app runs entirely in your browser — no installation, no internet required after the map tiles load.

---

## How to Open It

1. Download `bavaria_cop_leaflet.html`
2. Open **Chrome** or **Edge**
3. Drag the file into the browser window — or double-click it
4. The map loads centered on the 1809 theater between Donauwörth and Passau

> **Note:** You need an internet connection the first time you open it so the map tiles can load. After that the tiles cache and it works offline.

---

## The Map

- Real **OpenStreetMap** street map of Bavaria
- Centered on the operational area: Donauwörth → Regensburg → Straubing → Landshut
- **Scroll wheel** to zoom in and out
- **Click and drag** to pan
- **Hover over any town dot** to see the town name

---

## Pre-Loaded Units

All units start at their historical positions on **16 April 1809 at 0600**:

| Unit | Starting Position | Faction |
|---|---|---|
| Napoleon | Donauwörth | French |
| Davout HQ | Regensburg | French — III Corps |
| Morand, Saint-Hilaire, Gudin, Friant, Demont | Regensburg | French — III Corps |
| Montbrun, Saint-Sulpice | Regensburg | French — III Corps CAV |
| Vandamme HQ | Weihmichl | French — VIII Corps |
| Württemberg Cav, Württemberg Inf, Nansouty | Weihmichl | French — VIII Corps |
| Hiller | Landshut | Austrian — VI Corps |
| Charles HQ, Hohenzollern, Rosenberg, Bellegarde | Straubing | Austrian — Hauptarmee |

---

## The Clock

The game clock is in the top bar showing the current DTG in the format **DD HHMM APR**.

| Button | Action |
|---|---|
| −1H | Step back 1 hour |
| −30M | Step back 30 minutes |
| +30M | Advance 30 minutes |
| +1H | Advance 1 hour |
| Speed selector | Set playback speed (1×, 5×, 30×, 60×) |
| ▶ PLAY | Run the clock forward automatically |
| ⏸ PAUSE | Stop the clock |

When the clock advances, all units with active move orders automatically move along their routes. Units arrive at their destinations automatically when elapsed time equals travel time.

---

## The Four Tabs

### PLACE Tab — Add and Remove Units

**To place a unit using the dropdown:**
1. Select **FRENCH** or **AUSTRIAN** faction
2. Pick a unit from the unit dropdown
3. Pick a town from the location dropdown
4. Click **📍 PLACE**

**To place a unit by clicking the map:**
1. Select faction and unit from the dropdowns
2. Click **🗺 CLICK MAP** — the button turns green and the cursor becomes a crosshair
3. Click anywhere on the map
   - Click **near a town** — unit snaps to that town automatically
   - Click **in open terrain** — unit places at that exact field position
4. Click-place mode cancels automatically after placing

**To remove a unit:**
1. Click the unit on the map or select it from the UNITS tab
2. Click **✕ REMOVE SELECTED**

---

### MOVE Tab — Issue Move Orders

1. Select the unit you want to move from the dropdown
2. Pick a destination town
3. Enter the departure time in format **DD HHMM** (e.g. `16 0800` for 16 April at 0800)
4. The app automatically calculates:
   - Distance in km (as the crow flies)
   - Travel time based on unit type and speed
   - ETA at destination
5. Click **⚡ ISSUE MOVE ORDER**
6. A dashed line appears on the map showing the planned route
7. As the clock advances the unit dot moves along the line

**To cancel a move order:** Select the unit and click **✕ CANCEL MOVE ORDER**

**Unit speeds used for ETA calculation:**

| Type | Speed |
|---|---|
| Napoleon / Army HQ | 8 km/hr |
| French cavalry | 5 km/hr |
| French infantry HQ | 5 km/hr |
| French line infantry | 4 km/hr |
| Austrian cavalry | 4 km/hr |
| Austrian infantry | 3 km/hr |

---

### UNITS Tab — View All Units

- Shows every placed unit with current location and move order status
- Use the filter box to search by name
- Click any unit in the list to select it and center the sidebar on it
- Units moving show an arrow: **→ Destination**

---

### INTEL Tab — Contact Alerts and Log

**Contact Alerts** fire automatically when any French unit comes within **20 km** of any Austrian unit. The alert shows both unit names and distance.

**Movement Log** records every action taken during the session with a timestamp — placements, move orders, cancellations.

---

## Clicking Unit Markers on the Map

Click any unit marker on the map to open a popup showing:
- Unit name and color
- Faction and corps
- Unit type and speed
- Current location
- Destination, departure time, and ETA (if a move order is active)

---

## Town List

All towns in the theater are pre-loaded with accurate GPS coordinates. Hover over any gold dot on the map to see the town name. Key towns include:

**Along the Danube:** Donauwörth, Neuburg, Ingolstadt, Vohburg, Kelheim, Regensburg, Straubing, Plattling, Deggendorf, Passau

**Central corridor:** Abensberg, Rohr, Rottenburg, Pfeffenhausen, Mainburg, Eggmühl, Langquaid, Schierling, Ergoldsbach, Neufahrn

**South:** Landshut, Moosburg, Freising, Erding, Dachau, Munich

**East (Austrian approach):** Braunau, Burghausen, Mühldorf, Neu Oetting, Eggenfelden, Dingolfing, Landau

---

## Tips for Classroom Use

- **Umpire** can use this as the master COP, updating unit positions as reports come in
- **Players** can use it to plan move orders and calculate ETAs before writing formal orders
- The **contact alert** system gives early warning of converging forces
- Use the **PLAY** button at 30× or 60× speed to fast-forward through a march and see where units will be at a given time
- The **Movement Log** in the INTEL tab keeps a running record of all actions — useful for after-action review

---

## Technical Notes

- Built with **Leaflet.js 1.9.4** and **OpenStreetMap** tiles
- No server required — runs as a single HTML file
- Tested in Chrome and Edge
- Distance calculations use straight-line (as the crow flies) measurement
- Unit speeds are based on historical march rates from the Flight of the Eagle ruleset

---

## Credits

Built to support the **Flight of the Eagle — 1809 Danube Campaign** wargame at the U.S. Army War College, Carlisle Barracks, PA.

Historical source material: John H. Gill, *From Abensberg to Znaim: the Franco-Austrian War of 1809* (USAWC monograph, 2026); Jay Luvaas, *Napoleon on the Art of War* (Free Press, 1999); Napoleon's historical correspondence, Germany 1809.

---

*This tool is for educational use in support of USAWC professional military education.*
