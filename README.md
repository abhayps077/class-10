# Class 10 chapter PDF bundle

This folder is a standalone handoff bundle. The TeacherMate project was not changed.

## Contents

- `pdfs/class10/<book>/ch01.pdf`, `ch02.pdf`, and so on: chapter PDFs copied from `D:\LOST.DIR`.
- `class10-books.json`: catalog with subjects, book names, chapter numbers, URLs, and original filenames.
- `class10-books.ts`: the same catalog as a TypeScript constant for importing into an application.

The bundle contains 11 NCERT books and 92 chapter PDFs. Cover pages, answer keys, appendices, and preface PDFs are intentionally excluded. Original PDFs in `D:\LOST.DIR` were not changed. Chapter titles are numbered placeholders; the source PDFs retain their original chapter text and the actual names are recorded in `sourceFile` when they differ.

## Copying PDFs into TeacherMate later

Copy the contents of this bundle's `pdfs\class10` directory into the TeacherMate project's `public\pdfs\class10` directory. The catalog `pdf` values then resolve as browser paths such as `/pdfs/class10/science/ch01.pdf`.

The TypeScript catalog is descriptive asset data, not a database seed. Before importing records into TeacherMate's Supabase database, map each book and subject to the IDs in that project's database and connect each chapter PDF URL to its resource record. This avoids assuming IDs or changing the existing database.

## Subject and book mapping

- Mathematics: Mathematics Textbook for Class 10
- Science: Science Textbook for Class 10
- Social Science: History, Geography, Political Science, Economics (separate books)
- English: First Flight; Footprints Without Feet
- Hindi: Kshitij - Part 2; Kritika - Part 2
- Sanskrit: Shemushi - Part 2
