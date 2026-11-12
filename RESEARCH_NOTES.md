# Research notes: historical mechanics behind the Compendium

The site is a contemporary synthesis. Its objects draw from different dates, makers and cultural contexts; they are not presented as one authentic historical collection.

## Astronomical compendium

A documented 1575 Humfrey Cole compendium combined a nocturnal, latitude list, universal equatorial sundial, compass and perpetual calendar. The specific instrument had a suspension ring and was made as a compact portable object. This supports the overall concept of one body containing multiple coordinated functions.

Reference: Oxford History of Science Museum / EPACT, Astronomical Compendium signed by Humfrey Cole, dated 1575.
https://www.mhs.ox.ac.uk/epact/catalogue.php?ENumber=62715&Level=Detail

## Volvelle

The archive index borrows the layered, independently rotating paper-instrument principle. Here, each register is explicitly assigned a different archive variable: division, year and research volume. This is a contemporary use of the mechanism rather than a claim that historical volvelles were used as website menus.

The previous supplied implementation already established the three-ring concept and shared state; the new version preserves and extends that idea.

## Planispheric astrolabe

The mater holds one or more latitude plates. The rete is an openwork star map carrying star pointers and the ecliptic; it rotates freely above the tympan. The front's operation depends on stereographic projection. Different latitudes require different horizon plates unless a universal or single-latitude design is used.

References:
- Whipple Museum, The Parts of an Astrolabe: https://www.whipplemuseum.cam.ac.uk/explore-whipple-collections/astronomy/medieval-astrolabe/parts-astrolabe
- Museo Galileo, Astrolabe Components: https://catalogue.museogalileo.it/indepth/AstrolabeComponents.html
- Smithsonian, Persian Planispheric Astrolabe: https://www.si.edu/object/persian-planispheric-astrolabe%3Anmah_997139

Solar calculations use NOAA's published approximate equations for equation of time, solar declination, true solar time, hour angle, zenith/altitude and azimuth.

Reference: NOAA Global Monitoring Laboratory, General Solar Position Calculations: https://gml.noaa.gov/grad/solcalc/solareqns.PDF

## Transit theodolite

A transit theodolite has separate horizontal and vertical graduated circles, read through verniers. A Smithsonian example describes a horizontal circle graduated in both directions and a vertical arc read by vernier, as well as telescope and stadia wires.

References:
- Smithsonian, Theodolite (1840s): https://www.si.edu/object/theodolite%3Anmah_747673
- Smithsonian, Transit Instrument: https://www.si.edu/object/transit-instrument%3Anmah_997288

The site's controls preserve the independent horizontal/vertical axes and calculate the line-of-sight vector. It does not claim a full vernier microscope simulation.

## Armillary sphere

An armillary sphere represents celestial great circles with rings: horizon, celestial equator, colures and ecliptic. The polar axis is adjusted to the observer's latitude. Depending on construction, armillaries served demonstration or actual observational measurement.

References:
- Oxford History of Science Museum, Armillary Sphere: https://www.hsm.ox.ac.uk/armillary-sphere
- EPACT, Armillary Sphere: https://www.mhs.ox.ac.uk/epact/article.php?ArticleID=1
- Museo Galileo, Armillary Sphere (1564): https://catalogue.museogalileo.it/object/ArmillarySphere_n02.html

## Polar–Amsler planimeter

A polar planimeter has a pole arm anchored at one end and a tracer arm connected at a pivot. The measuring wheel records the relevant component of movement. The Smithsonian explains the polar coordinate arrangement and gives the area relation `A = 2π × tracer-arm length × wheel radius × wheel revolutions`.

Reference: Smithsonian, Polar–Amsler Planimeter: https://www.si.edu/spotlight/planimeters/polar-amsler

The digital demonstration derives equivalent wheel turns from the area of the closed path. This is explicitly disclosed; it does not pretend to simulate the actual wheel's differential integration path.

## Nocturnal

Humfrey Cole's c.1575 nocturnal has a calendar scale, a volvelle carrying an hour scale, and an index arm marked `STELLA POLARIS` / `INDEX HORA NOCTIS`. The reverse includes a degree scale, 24-hour scale, compass rose and lunar-age disc with a moon-phase aperture.

Reference: Oxford History of Science Museum / EPACT, Nocturnal signed by Humfrey Cole, c.1575.
https://www.mhs.ox.ac.uk/epact/catalogue.php?ENumber=24134&Level=Detail

The website's nocturnal-inspired chronology uses a calendar and sidereal-time reference to make date/time selection meaningful. It clearly distinguishes calculated sidereal time from historical visual alignment on Polaris.

## Ramelli bookwheel

Ramelli's 1588 design was intended to let readers consult several books. The essential kinematic feature is that the book platforms remain level as the wheel rotates, achieved by a gear arrangement. RIT's engineering reconstruction notes that Ramelli's own design was not built during his lifetime, although later bookwheels existed.

Reference: Rochester Institute of Technology, Renaissance Bookwheel: https://www.rit.edu/carycollection/renaissance-bookwheel

The digital bookwheel uses counter-rotation of each cradle to preserve orientation. It is a kinematic interpretation, not an exact gear-train reconstruction.

## Renaissance studiolo

The Gubbio studiolo (c.1478–82) uses wooden intarsia to create illusionistic cupboards, shelves and objects. Its trompe-l'oeil surfaces create an architectural image of a private study. The website translates the fitted-cabinet idea into content-bearing compartments without falsely claiming the historical cabinets were digital drawers.

References:
- Metropolitan Museum of Art, Studiolo from the Ducal Palace in Gubbio: https://www.metmuseum.org/art/collection/search/198556
- Metropolitan Museum of Art, On the Gubbio Studiolo: https://www.metmuseum.org/it/perspectives/points-of-view-gubbio-studiolo
