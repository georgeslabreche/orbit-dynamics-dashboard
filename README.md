# Orbit Dynamics Dashboard

## Introduction
A GitHub page to simulate spacecraft orbits around a celestial body (starting with for v.1.0).

**Concerns:**
- Processing power needed to execute all calculations. It may be very sluggish to run in Javascript.

## v.0.1: Orbits
- **Input:** Orbit parameters raan, incl, argp, a, e, and M.
- **Output:** 3D graph with sphere representing earth and the resulting spacecraft orbit.
- **Technical challenge:** How do we implement the 3D graph? Do we use a jQuery library for 3D plotting or do we use [WebGL](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API/Tutorial/Getting_started_with_WebGL) and [WebGLEarth](http://examples.webglearth.com/#satellite).

**Considerations:**
- Learning curve will be smaller with jQuery.
- Should the spacecraft be animated in orbit?

**WebGL Resources:**
- [Geoid Viewer](http://geomatica.como.polimi.it/elab/geoid/geoidViewer.html)
- [CNES Satellites](https://experiments.withgoogle.com/search?q=satellite)

**jQuery Resources:**
- [jquery.earth-3d](http://sebastien.drouyer.com/jquery.earth-3d/)
- [Differential Equation Solver](https://github.com/littleredcomputer/odex-js)
- [ODE Solver with Numeric Javascript](http://www.numericjs.com/workshop.php?link=fdd38094da018f6071cb2d51d47c7fb3de869cb5dd0b4f3b677b480ce7ffbd31)
- [Another ODE Solver](http://llarsen71.github.io/GMA1D/Docs/files/ODE-js.html)

## v.0.2: Groundtracks
- World map displaying groundtrack of the spacecraft.

**Considerations:** 
- Could also trace the groundtrack on the sphere's surface as the spacecraft is orbiting above. 

## v.0.3: Elevation and Azimuth
- The user can select a ground station on the grountrack map by clicking anywhere on the map.
- Selecting a ground station will generate the azimuth and elevation graphs.

**Considerations:**
- Need to put some thought into the workflow and user experience.

## v.0.4: LOS
- Satellite line of sight circle of for the selected groundstation.

## v.1.0: Prettified
Make pretty. Work on look and feel, polish things up.
