# images/

Web-ready photos used by the gallery in **Teaching → Off the page**.
All are 1200×900 (4:3), JPEG quality 82 — about 1.9 MB for the whole set of 12,
laid out as a 4×3 collage on desktop and 6×2 on mobile.

| File | What it shows |
| --- | --- |
| `teaching-spanish-reader.jpg` | Teaching from a Spanish graded reader (projected) |
| `picture-books-classroom.jpg` | Laying out picture books, Taipei classroom |
| `spanish-graded-readers.jpg` | The graded readers on a shelf |
| `haitian-program-chile.jpg` | A student and his certificate, Haitian immigrant programme, PUC Santiago |
| `lexicultural-stamps.jpg` | Student photographing the JAPÓN stamp panel, Santiago post office |
| `lexicultural-outing.jpg` | Japanese students at the stamp displays, Santiago |
| `conference-talk.jpg` | Presenting the illustrated-books study |
| `ntust-afl-team.jpg` | Applied Foreign Languages colleagues, NTUST |
| `coaching-soccer.jpg` | Coaching the FCBase Taiwan girls |
| `soccer-medal.jpg` | Second place, coaching season |
| `coaching-basketball.jpg` | Basketball drill, Glory Days Sports |
| `glory-days-sports.jpg` | Youth basketball league court |

Keeping the count a multiple of three keeps the desktop grid square. If you add
a thirteenth, either add two more or drop one.

## Children's faces

Every identifiable minor in these photos has been **irreversibly anonymised** —
the face region is downsampled to a coarse mosaic and then smoothed, so the
detail is destroyed in the file itself, not merely hidden. Blurred: 2 faces in
`picture-books-classroom`, 4 in `coaching-soccer`, 1 in `coaching-basketball`,
1 in `glory-days-sports`.

If you swap in new photos, keep this rule. The site says so out loud under the
gallery, and that promise should stay true.

## originals/

Your full-resolution camera files (HEIC/JPG/MOV, ~167 MB) live in `originals/`,
which is **git-ignored** — they stay on your machine and never enter the repo's
history. Note that HEIC does not display in browsers, so anything from an iPhone
must be converted before it can go on the site.

To regenerate or add photos, the processing script is straightforward: load,
apply EXIF rotation, anonymise any faces, crop to 4:3, resize to 1200×900, save
as progressive JPEG at quality 82.
