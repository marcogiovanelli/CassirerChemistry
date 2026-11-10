# Proofreading and citation report

The English prose of `CassirerChemistry.tex` has been proofread in place. The review made 76 small corrections or reductions, including grammar, punctuation, idiom, a missing closing parenthesis, and unnecessary repetition. English translations were corrected where the change was grammatical and did not alter their meaning. Debatable terminology and substantive attributions remain unchanged below.

The manuscript was found in `/Users/marco/Documents/GitHub/CassirerChemistry`, rather than the reference-only ChatGPT project mirror. No commit or push was made.

## Length and verification

The revised limit is **12,000 words**. The paper is below this limit under each of the following checks:

- **9,758 words** in a customized TeXcount count of the prose, abstract, headings, and visible footnotes, excluding the bibliography, hidden original-language quotation arguments, suppressed notes, comments, and mathematical expressions. Custom title and citation macros were accounted for.
- Approximately **10,873 alphabetic words** in the compiled PDF, including citation text and the bibliography.
- **11,585 whitespace-separated tokens** in the compiled PDF, a broader count that also includes dates, page numbers, and formulas. PDF extraction and hyphenation make these latter two figures approximate.

Exact preservation checks passed for the preamble, LaTeX command sequence and braces, citation keys and locators, cross-references, URLs, mathematical expressions and equation environments, direct quotations, original-language text in translated quotations, foreign-language terms, existing comments, paragraph divisions, and section structure. The bibliography and style file are unchanged.

An isolated build completed successfully, including bibliography processing, with no unresolved citations or cross-references. The existing document setup still produces minor warnings about the `submitted` option, margin notes, Latin bibliography localization, a PDF bookmark, and one line extending about 2.2 points beyond its margin. The manuscript's formatting commands were preserved. The compilation was used for verification; the existing PDF in the repository was not replaced.

## Passages and existing syntax left for author review

Line numbers below refer to the edited manuscript; the line and paragraph divisions were preserved.

| Line | Passage | Reason for leaving it unchanged |
|---|---|---|
| 49 | `\cite[\VD1{8}{121}]{ECN}` | The style defines `\VD` with two arguments. This invocation renders **“Vol. 1, Doc. 8121”**, rather than the likely intended volume 18, document 121. Review the invocation. The existing date conflict in the adjacent `\todo` cannot be settled without the letter scan. |
| 54 | The unparenthesized `\letterecnd` following “the book” | This produces “the book Cassirer to Meyerson, Jan. 1, 1910” in running text. A parenthesized reference may be intended, but the command and citation structure were preserved. |
| 56 | “a rather well-informed twenty-page section” | The section spans German pp. 270–292 and approximately eighteen pages in the cited translation. “Twenty-page” may be an approximation; “well-informed discussion” would also be more natural. No revision was imposed. |
| 109 | Mitscherlich footnote | “Chemical compounds with the same number of atoms form the same type of crystal shape” is grammatically intelligible but a broad technical formulation. A substantive revision would exceed proofreading. |
| 139 | “the absolute values of the relative atomic weights” | “Absolute values” can suggest a mathematical operation, whereas determinate values on a relative scale may be intended. Terminology was preserved. |
| 175 | Closing translated fragment | The German argument contains more material than the final English fragment alone, partly translated in the preceding direct quotation and prose. Its closing phrase about representation according to general rules is not explicitly rendered. No missing substantive content was supplied. |
| 183 | German `o greift diese Forderung ...` | The scan reads “so greift ...”; the supplied original appears to lack its initial `S`. Non-English text remains exact. |
| 188 | `\citep[see][e.g.]{Arnesano2025}` | “e.g.” occupies the citation's postnote field. Review whether “see, e.g.” was intended entirely as a prenote. Citation arguments were preserved. |
| 190 | `\citep[see][6.III]{Cassirer1907}` | The bibliography key `Cassirer1907` identifies the 1906 *Probevorlesung*, reprinted at pp. 3–16, rather than the 1907 second volume of *Das Erkenntnisproblem*. Check that this is the intended key and locator. |
| 194 | “relative resting-point” | The quotation occurs on printed p. 292, but there it characterizes the atom as a relative pause in a dynamic process. Its application here to convergence on new numerical constants is an interpretation, rather than the literal wording of that passage. |
| 228 | `\qt{limit-concept} (\emph{Grenzbegriff})` | `\qt` requires two mandatory arguments. Here it consumes the opening parenthesis as its second argument, visibly leaving an unmatched closing parenthesis after *Grenzbegriff*. Correcting the invocation would alter protected LaTeX syntax. |
| 334 | “Nevertheless, Cassirer identifies ... in Cassirer's historical reconstruction” | The context strongly suggests that the first name should be **Meyerson**. The named attribution was left for author review. |
| 336 | “functional legality” | “Lawfulness” may be more idiomatic if this renders *Gesetzlichkeit*, but changing philosophical terminology requires authorial judgment. |
| 344 | German `übeundifferentiatedr` | This is visibly corrupted, probably for `über`. The original-language text remains unchanged. |
| 357 | Identification of the reply to Doc. 195 | The existing note contrasts the letters of 23 June and 7 April 1913. No resolution was assumed without the scans. |
| 361 | “the constancy of a numerical ratio” / *Maßbegriff* | Whether “numerical ratio” captures the intended concept of measure is a substantive interpretive choice. |
| 371 | “defined strictly substantially”; “quantity-definite numerical relations” | These translated expressions remain awkward, but their revision could alter the contrast between *Was* and *Wieviel*. Consider reviewing them against the published translation. |

## Citation checks against attached sources

Printed page numbers were used. The attached Cassirer volume is the German 1910 edition; English numbers after a slash could not be checked without the English translation. The attached Meyerson scan is the 1908 French edition. The Duhem book is Needham's English translation, whose bracketed markers explicitly preserve the French original's pagination.

### Discrepancies and qualifications

| Manuscript location | Finding |
|---|---|
| Line 77: `\citet[71]{Duhem1902}` | Richter's acid/base series and their associated masses occur on original **p. 69**, with the setup on **p. 68**. These are English printed pp. 43–44 in the attached translation. Original p. 71 discusses Dalton's multiple proportions. Review **69** or **68–69** in place of 71. This check uses the translation's original-page markers, rather than images of the French original. |
| Line 137: “comparison sequence” / `gemeinsame Vergleichsreihe`, in a paragraph citing `\SF{277}{208}` | The exact German expression occurs on printed **p. 254**, in the discussion of energy. Printed p. 277 supports the analogous coordination of property series through the atom-concept, but does not contain this wording. Consider a separate citation to p. 254 or review the quotation's placement. The corresponding English locator was not verified. |
| Line 214: `\SF{292}{220}` after the concern with an individual element or compound | Printed p. **292** supports the methodological contrast between universal and particular. The explicit formulation about the chemical **Einzelding** and its properties is on printed **p. 271**. The current reference is relevant, but 271 is the more direct locator for that sentence. |
| Line 73: `\cite[see][III]{Duhem1902}` | Richter is discussed in **Part II, chapter III**. The bare “III” is ambiguous because Part I also has a chapter III, on the Newtonian school. |
| Line 309: commented-out figure citation `\cite[139]{Duhem1902}` | If this figure is restored, the enantiomer diagram is on original **p. 129**, English printed **p. 83**; original p. 139 concerns criticism of valence. The existing comment is untouched. |

All citation numbers and keys remain unchanged in the manuscript, including the discrepancies above.

### Confirmed locators

The following German Cassirer locators were checked for the cited wording or subject. Confirmation concerns page location, not endorsement of every interpretive claim made in the paper.

| Printed pages | Located material |
|---|---|
| 189–190 | Duhem, Regnault, and the theoretical interpretation of measurements of gases. |
| 204–205 | Qualities treated as transferable entities, phlogiston, and the “excellent presentation” footnote. |
| 214 | The dissolution of the material atom into a system of electrons. |
| 270–272 | Chemistry's methodological position, mathematical laws, *Einzelding*, historical approach, and numerical determination. |
| 273–275 | Richter's series, independence from atomism, combining versus atomic weight, underdetermination, and convergent physical criteria. |
| 276–280 | Atom as goal, coordination of property series, scientific production versus critical reflection, the atom as Idea and form-concept. |
| 281–285 | Substitution, valence, types, Dumas and Regnault, mathematical versus empirical equivalence, and constitutional formulas. |
| 286–287 | Laurent and Gerhardt, radicals, relations between initial and final states, characteristic numbers, and the numerical domain. |
| 289–292 | Periodic ordering, Locke, nominal and real essences, prediction, variable atomic weights, and the relative resting-point. |
| 298–299 | The long quotation about constitutional formulas, chemical types, and the increasing distinction of isomers. |
| 304–307, 309 | Limit-concepts, *Einzelheit* versus *Dinglichkeit*, numerical constants and the particular, and inexhaustibility. |
| 430–431 | The discussion of Meyerson near the end of the book. |

Two source notes should be kept distinct: Cassirer **p. 205** cites Meyerson **pp. 300ff.** as an “excellent presentation”; Cassirer **p. 272** separately cites Meyerson **pp. 213ff.** The existing `\todo` accurately identifies the latter reference, but the two notes play different roles.

Additional confirmations:

- **Meyerson 1908, p. 203**: the phlogiston/Lavoisier discussion is present; p. 204 continues the point.
- **Meyerson 1908, chapter VII**: *L'unité de la matière*, printed pp. **213–235**, is relevant to the discussion of unification; the closing argument is particularly explicit at pp. 231–235.
- **Duhem 1902, Part II, chapter VII**: isomerism and stereochemistry, original pp. **123–132**, English printed pp. **78–84**.
- Cassirer's footnotes themselves cite **Meyer p. 176** at printed p. 289 and **Wurtz p. 175** at printed p. 284. This confirms agreement with Cassirer's citations, but does not independently verify the pages in those books.

### Locators not independently verifiable from the attachments

| Work | Unverified manuscript locators |
|---|---|
| Cassirer 1907b | 312–313. |
| Cassirer 1911a | Vol. 2: 428–441, 433, 434, 435, 440. |
| Cassirer 1921 | 17, and English 359–360. |
| Cassirer 1929 | 505/433, 516/442–443, 520/446. |
| Cassirer 1936 | 107–108/85–86; 178/143; 179/144; 183–184/147; 184–186/148–150; 186/149; 187/150; chapter IV.2. |
| Cassirer 1910, English translation | All English page numbers after slashes. |
| Meyerson 1911 | 100, 101, 102, 103, 122–123, 123 and fn. 1, 129. |
| Meyerson 2011 | 195–197. |
| Ladenburg 1902 | 175, 189ff., 122–124, 274–278, and lecture references. |
| Ostwald 1906 | 44–49 and lecture references. |
| Wurtz 1879; Meyer 1884 | 175; 176, respectively, except for the indirect agreement noted above. |
| Bensaude-Vincent and Telkes-Klein 2016 | 31. |
| Perrin 1910 | 281. |
| ECN correspondence | Document numbers, letter dates, and quoted wording require the absent letter scans. |

The attached *Atomic Notation and Atomistic Hypotheses* is a different Duhem work, translated from his 1892 article. It cannot verify locators in *Le mixte* or *La théorie physique*. The latter work is not attached.
