# Word2vec for Akkadian

The present repository provides notebooks and files for drawing lemmatized Akkadian words out of [ORACC](http://oracc.org) projects. The purpose of this is to test word2vec on Akkadian vocabulary. 

# The Corpus
The texts that are used come from different periods and represent different text types. The text categories may be described by [ORACC](http://oracc.org) project:

## Royal Inscriptions
* [RINAP](http://oracc.org/rinap): Neo-Assyrian royal inscription (ca. 900-612 BCE)
* [RIAO](http://oracc.org/riao): Earlier Assyrian royal inscriptions (ca. 1900-100 BCE)
* [RIBO](http://oracc.org/ribo): Babylonian royal inscriptions (ca. 1100-64BCE)
* [SUHU](http://oracc.org/suhu): Royal inscriptions of two early first-millennium-BC rulers of the kingdom of Sūḫu

The [RINAP](http://oracc.org/rinap) and [RIBO](http://oracc.org/ribo) projects are further subdivided according to king (RINAP) or dynasty (RIBO).

## Technical, scholarly, religious, and literary texts
* [GLASS](http://oracc.org/glass): Middle Babylonian (ca. 1200 BCE) and Neo-Assyrian (ca. 625 BCE) technical recipes for the production of glass and perfumes.
* [CAMS/GKAB](http://oracc.org/cams/gkab): Neo-Assyrian (ca 800-612BCE) and Late Babylonian (ca. 300BCE) scholarly libraries from Nimrud, Huzirina, and Uruk.
* [CCPO](http://ccp.yale.edu): Neo-Assyrian (ca. 650BCE) and Late Babylonian (ca. 300 BCE) scholarly commentaries on traditional texts.
* [CMAWRO](http://oracc.org/cmawro): Old Babylonian (ca. 1800 BCE) and first millennium anti-witchcraft texts.
* [CAMS/ANZU](http://oracc.org/cams/anzu): Reconstruction of the first millennium version of the three tablets (chapters) of the Anzu story.
* [BLMS](http://oracc.org/blms): First millennium bilingual (Sumerian - Akkadian) texts from Babylonia and Assyria. Includes cultic songs, literary texts, and incantations.

Several of these projects include both Sumerian and Akkadian (often in the same document). For the purpose of this project only the Akkadian is included in the output.

## Letters and Adminstrative Texts
[AEMW/AMARNA](http://oracc.org/aemw/amarna): International correspondence of the Egyptian Pharaoh found in Amarna, ca 1300 BCE.
[HBTIN](http://oracc.org/hbtin): Hellenistic-period contracts from Uruk.
[SAAO](http://oracc.org/saao): letters and administrative texts from the Assyrian royal court (ca. 800-612 BCE).

The [SAAO](http://oracc.org/saao) project is subdivided into 19 sub-projects according to the volumes in the SAA series. Each volume includes letters or documents relating to a particular king, or is devoted to a particular subject (such as divination). In the current output all SAAO documents are found in a single file.

A few projects have not been included here, for a variety of reasons. [DCCMT](http://oracc.org/dccmt) and [RIMANUM](http://oracc.org/rimanum) are in need of updating. The lexical texts in [DCCLT](http://oracc.org/dcclt) do not provide a regular textual context and may therefore be less valuable for word2vec (one could argue, similarly, that the commentary texts in [CCPO](http://oracc.org/ccpo) should not be included. It might be worth adding [DCCLT](http://oracc.org/dcclt) and [DCCLT/NINEVEH](http://oracc.org/nineveh) to see how this changes the outcomes of the analysis.

In collecting the data from [ORACC](http://oracc.org) only lemmatized texts have been taken into account. For an introduction to ORACC lemmatization see the [documentation page](http://oracc.museum.upenn.edu/doc/help/lemmatising/primer/).

# Data and Data Format
Each `.csv` file in `/output` has two fields: `id_text` and `lemma`
