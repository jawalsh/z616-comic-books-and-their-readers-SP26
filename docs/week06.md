{% include_relative header.md %}

[acrobat]: https://iuware.iu.edu "Adobe Acrobat on IUWare"
[finereader]: https://pdf.abbyy.com "ABBYY FineReader"
[tesseract]: https://tesseract-ocr.github.io/tessdoc/Installation.html "Tesseract docs"

# Week 6: Fan mail and corpus-building

## Summary
This week we will explore the topic of comic book fan mail and learn techniques for building a corpus of fan mail for research investigations.  

## Weekly Learning Objectives
- *define* key terms, such as *letter of comment*, *letterhack*, and *text analysis*.
- *discuss* scholarship on comic books fan mail and other paratexts.
- *express* basic concepts and goals of computational text analysis.
- *analyze* a small set of fan mails examples from different decades.
- *use* software tools to convert images of comic book fan mail into searchable digital text. 

## Before class: Readings, resources, and tasks

### Readings

* [Comic book letter column.](https://en.wikipedia.org/wiki/Comic_book_letter_column). _[Wikipedia.](http://wikipedia.org/)_. <!-- 8 pp. -->
* [Letterhack.](https://en.wikipedia.org/wiki/Letterhack). _[Wikipedia.](http://wikipedia.org/)_. <!-- 1 pp. -->
* Misemer, L. (2020). [Reading Comics at the Threshold: A Round Table on Letter Columns & Other Comics Paratexts (Part 1).](https://themiddlespaces.com/2020/09/15/reading-comics-at-the-threshold-part-1/). [The Middle Spaces: Comics. Music. Culture.](https://themiddlespaces.com/) <!-- 9 pp. -->
* Kashtan, A. (2020). How can a comic book’s use of paratexts help it appeal to young readers? in [Reading Comics at the Threshold: A Round Table on Letter Columns & Other Comics Paratexts (Part 3).](https://themiddlespaces.com/2020/09/29/reading-comics-at-the-threshold-part-3/). Ed. L. Misemer. [The Middle Spaces: Comics. Music. Culture..](https://themiddlespaces.com/) <!-- 8 pp. -->
* Shoemaker, M. (2020). [Text Analytics.](https://guides.temple.edu/c.php?g=78518&p=505212). Temple University Libraries.
* Wermer-Colan, A. (2020). [Computational Textual Analysis.](https://guides.temple.edu/corpusanalysis). Temple University Libraries.
* Walsh, J. A., Martin, S., & St. Germain, J. (2018). [“The Spider’s Web”: An analysis of fan mail from Amazing Spider-Man, 1963–1995](https://f001.backblazeb2.com/file/gnrlfs/tr/Walsh+et+al+2018.pdf). In J. Laubrock, J. Wildfeuer, & A. Dunst (Eds.), _Empirical comics research: Digital, multimodal, and cognitive methods_ (pp. 62-84). New York: Routledge. <!-- 23 pp. -->

#### Recommended but optional reading
* Walsh, J. A, Martin, S., & St. Germain, J. (2017) [“The Spider’s Web”: An analysis of fan mail from _Amazing Spider-Man_, 1963–1995](https://f001.backblazeb2.com/file/gnrlfs/tr/walsh2017.pdf). Poster presented at the Comics Arts Conference / Comic-Con International, San Diego, CA, July 22, 2017.
* Underwood, T. (2015). Seven ways humanists are using computers to understand text. Retrieved from [https://tedunderwood.com/2015/06/04/seven-ways-humanists-are-using-computers-to-understand-text/.](https://tedunderwood.com/2015/06/04/seven-ways-humanists-are-using-computers-to-understand-text/) <!-- 9 pp. -->

### IT Skills

#### Converting a scan to searchable text with Adobe Acrobat
- [LinkedIn Learning: “Acrobat DC Essential Training: Convert a scan to searchable text](https://www.linkedin.com/learning/acrobat-dc-essential-training-2021/convert-a-scan-to-searchable-text)


#### Screenshots (Windows)


- <https://techcommunity.microsoft.com/t5/windows-11/how-to-take-a-screenshot-in-windows-11-4-ways/m-p/2849736>.
- <https://support.microsoft.com/en-us/windows/use-snipping-tool-to-capture-screenshots-00246869-1843-655f-f220-97299b865f6b>
- <https://support.microsoft.com/en-us/office/copy-the-window-or-screen-contents-98c41969-51e5-45e1-be36-fb9381b32bb7>

#### Screenshots (Mac)

*   <https://support.apple.com/en-us/HT201361>.

#### Screenshots (iPadOS/iOS)

*   iPadOS: <https://support.apple.com/en-us/HT210781>.
*   iOS: <https://support.apple.com/en-us/HT200289>.

#### Public Domain Comics / Downloadable Comics

*   [Digital Comic Museum.](http://digitalcomicmuseum.com/)(DCM)
*   [Comic Book +.](https://comicbookplus.com/)
*   [Internet Archive](http://archive.org/)

#### Tools used for today’s activities
* [Adobe Acrobat][acrobat] (Part of Adobe Creative Cloud, available at <https://iuware.iu.edu>.)
* [ABBYY FineReader][finereader]
* [Tesseract][tesseract]
* [qpdf](https://qpdf.sourceforge.io)


## In class

- Lecture and tech demo
- Creating screen shots
- Performing OCR with [Adobe Acrobat][acrobat], [ABBYY FineReader][finereader], and [Tesseract][tesseract]
- Exploring fanmail activity
- Discussion

### Exploring fanmail activity

We will spend time in class individually looking for interesting examples of fan mail. Try to find two or three distinct examples. 

Keep notes on:

- Source of the fan mail: title, issue, date;
- topics discussed, e.g., story, plot, dialogue, art, characters, creators, process, current events, mistakes, criticisms, etc.;
- details the writers reveal about themselves, e.g., gender, occupation, etc.

After working individual, we will get together in small groups to share our findings, and then groups will report back to the full class.

#### Sources for finding fan mail
- comics in our shared OneDrive folder
* [Digital Comic Museum](http://digitalcomicmuseum.com/) (DCM)
* [Comic Book +](https://comicbookplus.com)
* [Internet Archive](http://archive.org)


