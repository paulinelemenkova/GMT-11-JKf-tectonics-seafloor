# GMT Tectonics and Seafloor Fabric — Global Plate Tectonic Map

A GMT (Generic Mapping Tools) shell script that draws a comprehensive global tectonic map combining plate boundaries, plate kinematics, seafloor fabric and subduction-zone geometry on a single equal-area world projection. The script has been used to generate tectonic map figures in the author's marine-geophysical and cartographic publications.

## What the script maps

- Tectonic plate boundaries for all major plates (Pacific, Philippine Sea, African, Antarctic, Arabian, Australian, Caribbean, Cocos, Eurasian, Indian, Juan de Fuca, Nazca, North American, Scotia, South American, Somali, Okhotsk), each colour-coded (psxy)
- Plate rotation (Euler) poles and plate-boundary steps from the PB2002 model (psxy with -i column selection)
- Global seafloor fabric from GSFML: fracture zones, discordant zones, extinct ridges, propagating ridges, V-shaped structures and other features (psxy)
- Global magnetic lineation picks (psxy)
- Subducting-slab depth contours for numerous subduction zones worldwide (Aleutians, Ryukyus, Central America, Caribbean, Philippines, Solomons, Vanuatu, Sulawesi, South Sandwich, South America, New Britain, Molucca, Mindanao, Luzon, Halmahera, Tonga and others), colour-scaled by depth
- Coastlines, plate labels, grid, scale bar and GMT logo (pscoast, pstext, psbasemap, logo)

The map uses the Eckert IV equal-area pseudocylindrical projection centred on the Pacific (180 degrees).

## Data sources

- Plate boundaries, rotation poles and steps: PB2002 model (Bird, 2003)
- Seafloor fabric and magnetic lineation picks: GSFML, Global Seafloor Fabric and Magnetic Lineation Data Base Project (SOEST, University of Hawaii)
- Subducting-slab contours: regional slab depth contour datasets
- Coastlines: GSHHG via GMT

## Requirements

- GMT 6.x (Generic Mapping Tools): https://www.generic-mapping-tools.org
- A POSIX shell (bash/sh)
- The PB2002, GSFML and slab-contour data files available locally

## Usage

Place the required tectonic / seafloor-fabric data files in the working directory, then run:

    bash GMT-11-JKf-tectonics-seafloor.sh

The script writes a PostScript file and converts it to a raster image (JPG/PNG) via psconvert.

## Author and citation

Polina Lemenkova
ORCID: https://orcid.org/0000-0002-5759-1089

This script supports figures in the author's marine-geophysical and cartographic papers; please cite the specific article a given figure appears in. The full publication list is available via the ORCID record above.

## License

See the LICENSE file in this repository.
