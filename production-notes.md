# Production notes

## Writer of the foreword
The forward “A Brief Life of Shakespeare” (`a-brief-life-of-shakespeare.xhtml`, `epub:type="foreword"`) is unsigned in the original scans. I have inferred that it was written by E. T. Roe (`wfw`) because the title page of the 1907 John A. Hertel Co. edition (from which the scans were sourced) reads “Edited and arranged by E. T. Roe, LL.B.”. The preface is signed “E. T. R.” and since “A Brief Life of Shakespeare” is also editorial apparatus of the same kind as the preface it seems logical that he also wrote it. 
Sources: title page of the page scans (https://archive.org/details/twentybeautifuls0000wmsh); Library of Congress name authority n83230843 (“Roe, E. T.”, variant “Roe, Edward Thomas”).

## Sources
- Transcription: Project Gutenberg ebook #1430 (1998), produced by Morrie Wilson, James Rose, and David Widger.
- Project Gutenberg’s HTML omits the Pronouncing Vocabulary of Names. However, it is included in the plain-text file and was sourced from there.
- Page scans: the complete Internet Archive scan of the 1907 John A. Hertel Co. edition (https://archive.org/details/twentybeautifuls0000wmsh). 

## Print text retained as printed
- The epitaph in “A Brief Life of Shakespeare” retains the exact spelling and formatting in the original text. `se modernize-spelling` does not modify quoted verse.

## Normalizations
- In the “Merit” citation the print reads “IV 1.” without a period; it is set as “IV. 1.” to match every other citation.
- The Pronouncing Vocabulary uses the print’s own notation (macrons, dot-below vowels, and prime stress marks); PG had substituted circumflexes and apostrophes.

## Editorial changes to the print
- “A Brief Life of Shakespeare”: the print’s “Thomas Nasbe” and “Thomas Quincy” are corrected to Thomas Nash and Thomas Quiney.
- Quotations: every citation was checked against the plays. Eleven misattributions in the print are corrected. This was done using code written with Claude code.
- Quotations, “Quarrels”: the print’s typo “these is no true valor” is corrected to “there is”.
- Quotations: two citations of “Love’s Labor Lost” are made “Love’s Labor’s Lost”, matching the third citation and the play’s title; the American spelling “Labor” is kept.
- Pronouncing Vocabulary: “Leodovico” and “Polixines” are corrected to “Lodovico” and “Polixenes”, the spellings used in the stories, and Lodovico’s pronunciation and alphabetical position are adjusted to match.

## Glossary
- The Pronouncing Vocabulary is marked up as a glossary with a search key map. The terms Cymbeline, Macbeth, Othello, and Pericles would share `id`s with the story files, so their glossary `id`s carry a `-glossary` suffix; the resulting `x-019` lint errors are ignored in `se-lint-ignore.xml`.
