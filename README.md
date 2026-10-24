# Class 10 chapter PDF bundle

This folder is a standalone handoff bundle. The TeacherMate project was not changed.

## Contents

- `pdfs/class10/<book>/<chapter-name>.pdf`: chapter PDFs copied from `D:\LOST.DIR`, named with descriptive chapter titles.
- `class10-books.json`: catalog with subjects, book names, chapter numbers and titles, PDF URLs, and original filenames.
- `class10-books.ts`: the same catalog as a TypeScript constant for importing into an application.

The bundle contains 11 NCERT books and 92 chapter PDFs. Cover pages, answer keys, appendices, and preface PDFs are intentionally excluded. Original PDFs in `D:\LOST.DIR` were not changed. The catalog keeps the original chapter number and title, while `sourceFile` records the original NCERT PDF filename.

## Copying PDFs into TeacherMate later

Copy the contents of this bundle's `pdfs\class10` directory into the TeacherMate project's `public\pdfs\class10` directory. The catalog `pdf` values then resolve as browser paths such as `/pdfs/class10/science/chemical-reactions-and-equations.pdf`.

The TypeScript catalog is descriptive asset data, not a database seed. Before importing records into TeacherMate's Supabase database, map each book and subject to the IDs in that project's database and connect each chapter PDF URL to its resource record. This avoids assuming IDs or changing the existing database.

## Subject and book mapping

- Mathematics: Mathematics Textbook for Class 10
- Science: Science Textbook for Class 10
- Social Science: History, Geography, Political Science, Economics (separate books)
- English: First Flight; Footprints Without Feet
- Hindi: Kshitij - Part 2; Kritika - Part 2
- Sanskrit: Shemushi - Part 2
