# Omega Sigma legacy site: content catalog

This catalog lists every event on the site, where its photos came from, and the copy used.
All site text lives in the `SITE` object near the bottom of `index.html`. To change a description, an officer, or an award, edit it there.

Chapter facts come from the official chapter page: https://www.ptk.org/chapters/omega-sigma-chapter

## How photos are organised

- Source: the "PTK" Google Drive folder, one subfolder per event.
- In the repo: `assets/photos/<event-slug>/01.jpg, 02.jpg, …`. Photos are converted from HEIC/PNG to JPG, resized to 1600px on the long edge, and rotated upright.
- `assets/photos/manifest.json` lists every file with its pixel size.
- To add a photo to an event: drop it in the event folder as the next number (e.g. `06.jpg`), then raise that event's `count` in `SITE.events`.
- To add a new event: create `assets/photos/<new-slug>/`, add numbered JPGs, and add an entry to `SITE.events`.
- The site shows photos in black and white to match the editorial design. Colour comes back on hover and in the photo viewer. The files themselves keep their colour.

## Events (in the order they appear on the site)

Dates come from the photos' camera timestamps.

| # | Event | Place | When | Photos used | Drive folder |
|---|-------|-------|------|-------------|--------------|
| 1 | Officer Induction | Houston | June 7, 2026 | 4 of 4 | Officer Induction |
| 2 | Honors Institute | University of Denver | June 20–22, 2026 | 5 of 12 | Honors Institute - University of Denver |
| 3 | Texas Honors Institute | Texas Junior College (to confirm) | July 10–11, 2026 | 5 of 10 (+2 videos not used) | Texas Honors Institute - Texas Junior College |
| 4 | First General Meeting | HCC – Northwest | September 4, 2026 (officer photos Aug 14) | 5 of 16 | First General Meeting |
| 5 | Fellowship | Around Houston | July–September 2026 | 5 of 9 | Fellowship |
| 6 | Second General Meeting | HCC – Northwest | October 2, 2026 | 4 of 7 (+1 video not used) | 2nd General Meeting |
| 7 | Texas Leadership Conference | Texas A&M University RELLIS Campus | October 9–11, 2026 | 6 of 19 | Texas Leadership Conference - Texas A&M Uni Rellis Camp |
| 8 | Third General Meeting | HCC – Northwest | November 6, 2026 | 4 of 6 | 3rd General Meeting |

### Descriptions

1. **Officer Induction**: The new officer team received their medallions in a backyard ceremony with advisors and friends, the quiet start of a busy year.
2. **Honors Institute, University of Denver**: Phi Theta Kappa's national Honors Institute brought our members to Denver for three days of lectures, seminars, and long conversations with chapters from across the country.
3. **Texas Honors Institute**: A summer weekend with chapters from across Texas: honors sessions by day, campus walks at dusk, and plenty of new friends from other colleges.
4. **First General Meeting**: The year's first general meeting introduced the officer team, welcomed new members, and gave everyone time to meet the advisors one-on-one.
5. **Fellowship**: Food-truck nights, coffee-shop planning sessions, and van rides to the next event. These are the in-between moments that turn a chapter into friends.
6. **Second General Meeting**: A hands-on meeting with a guest presentation, snacks, and members working through activities together around the room.
7. **Texas Leadership Conference**: Three days in Bryan–College Station for leadership workshops, sessions with chapters from across the state, and a visit to the George Bush Presidential Library.
8. **Third General Meeting**: A full room for the third meeting of the semester, as officers shared upcoming projects, opportunities, and ways for members to get involved.

## Where photos are also used

- Hero portrait: `fellowship/01.jpg` (officers with medallions on campus)
- Recognition block: `first-general-meeting/02.jpg`
- About strip: `honors-institute-denver/05.jpg`, `texas-leadership-conference/02.jpg`, `third-general-meeting/03.jpg`
- Officers banner: `officer-induction/02.jpg`

## Still needed from the chapter

- **Officers**: five names, roles, one-line bios, and a 3:4 portrait each (save as `assets/photos/officers/<role>.jpg` and set `photo` in `SITE.officers`). The roles are placeholders that follow PTK's usual President plus four hallmark VPs. Change them to match the real titles.
- **Texas Honors Institute location**: the Drive folder says "Texas Junior College". Please confirm the host college's exact name.
- **Not used**: three videos (`.MOV`), one large photo that the Drive download couldn't fetch (Texas Honors Institute, `8a3ffd43…jpg`, 6.6 MB), and a 7.6 MB PNG in Fellowship. `IMG_1529.HEIC` appears in both the Fellowship and Texas Leadership Conference folders (it's the same file).
