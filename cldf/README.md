<a name="ds-textcorpusmetadatajson"> </a>

# TextCorpus Multi-CAST Matukar Panau

**CLDF Metadata**: [TextCorpus-metadata.json](./TextCorpus-metadata.json)

**Matukar Panau** is a highly endangered Oceanic language spoken around 45 km north of Madang, Papua New Guinea. Although most children are no longer learning Matukar Panau, current speakers (approximately 300) form a vibrant community of multilinguals in dense social networks. As an Oceanic language on the Papua New Guinea coast, Matukar Panau has many interesting Papuan features.

The Multi-CAST Matukar Panau corpus constitutes a small subset of recordings made by Danielle Barth during her fieldwork between 2010–2020 (Australian National University Asia-Pacific Innovation Program Grant, *Resolving Ambiguity: What face-to-face communication can contribute*, PI: Danielle Barth); language documentation is ongoing. Data has been transcribed and translated with help from local community members, especially Kadagoi Rawad Forepiso and Rudolf Raward. Recordings can be found in the [ELAR](http://hdl.handle.net/2196/00-0000-0000-0012-388F-3) and PARADISEC ([1](http://catalog.paradisec.org.au/collections/DGB1), [2](http://catalog.paradisec.org.au/collections/SocCog)) archives. More information and resources on the language can be found on the [project website](https://matukar.wordpress.com/).

The texts in Multi-CAST were glossed with GRAID and RefIND by Danielle Barth, Kira Davey, and Maria Matheas. In addition to monologue narratives, some stimulus-based conversational descriptions have also been annotated with these schemata to enable research about referent expression when describing familiar and unfamiliar objects, places, and people. Recordings of these events are archived in ELAR and PARADISEC and those archives will eventually also provide open access to ELAN files with the annotations.

property | value
 --- | ---
[dc:bibliographicCitation](http://purl.org/dc/terms/bibliographicCitation) | Barth, Danielle & Davey, Kira & Matheas, Maria. 2023. Multi-CAST Matukar Panau. In Haig, Geoffrey & Schnell, Stefan (eds.), Multi-CAST: Multilingual corpus of annotated spoken texts. Version 2311. Bamberg: University of Bamberg. (multicast.aspra.uni-bamberg.de/#matukar) (date accessed)
[dc:conformsTo](http://purl.org/dc/terms/conformsTo) | [CLDF TextCorpus](http://cldf.clld.org/v1.0/terms.rdf#TextCorpus)
[dc:identifier](http://purl.org/dc/terms/identifier) | https://multicast.aspra.uni-bamberg.de/#matukar
[dc:license](http://purl.org/dc/terms/license) | https://creativecommons.org/licenses/by/4.0/
[dcat:accessURL](http://www.w3.org/ns/dcat#accessURL) | https://github.com/Multi-CAST/mcmatukar
[prov:wasDerivedFrom](http://www.w3.org/ns/prov#wasDerivedFrom) | <ol><li><a href="https://github.com/Multi-CAST/mcmatukar/tree/be7acde">Multi-CAST/mcmatukar be7acde</a></li><li><a href="https://github.com/glottolog/glottolog/tree/v5.1">Glottolog v5.1</a></li></ol>
[prov:wasGeneratedBy](http://www.w3.org/ns/prov#wasGeneratedBy) | <ol><li><strong>python</strong>: 3.12.3</li><li><strong>python-packages</strong>: <a href="./requirements.txt">requirements.txt</a></li></ol>
[rdf:ID](http://www.w3.org/1999/02/22-rdf-syntax-ns#ID) | mcmatukar
[rdf:type](http://www.w3.org/1999/02/22-rdf-syntax-ns#type) | http://www.w3.org/ns/dcat#Distribution


## <a name="table-utterancescsv"></a>Table [utterances.csv](./utterances.csv)

Annotated clauses of the texts in the collection.

property | value
 --- | ---
[dc:conformsTo](http://purl.org/dc/terms/conformsTo) | [CLDF ExampleTable](http://cldf.clld.org/v1.0/terms.rdf#ExampleTable)
[dc:extent](http://purl.org/dc/terms/extent) | 951


### Columns

Name/Property | Datatype | Description
 --- | --- | --- 
[ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string`<br>Regex: `[a-zA-Z0-9_\-]+` | Primary key
[Language_ID](http://cldf.clld.org/v1.0/terms.rdf#languageReference) | `string` | References [languages.csv::ID](#table-languagescsv)
[Primary_Text](http://cldf.clld.org/v1.0/terms.rdf#primaryText) | `string` | The example text in the source language.
[Analyzed_Word](http://cldf.clld.org/v1.0/terms.rdf#analyzedWord) | list of `string` (separated by `	`) | A grammatical word in the object language (or #, marking clause boundaries or ZERO marking zero anaphora). “Word” here should be understood in terms of a GRAID annotation unit.
[Gloss](http://cldf.clld.org/v1.0/terms.rdf#gloss) | list of `string` (separated by `	`) | The morphological glossing for the grammatical word, as per the Leipzig Glossing Rules. (or #, marking clause boundaries or ZERO marking zero anaphora).
[Translated_Text](http://cldf.clld.org/v1.0/terms.rdf#translatedText) | `string` | The translation of the example text in a meta language
[Meta_Language_ID](http://cldf.clld.org/v1.0/terms.rdf#metaLanguageReference) | `string` | References the language of the translated text<br>References [languages.csv::ID](#table-languagescsv)
[LGR_Conformance](http://cldf.clld.org/v1.0/terms.rdf#lgrConformance) | `string`<br>Valid choices:<br> `WORD_ALIGNED` `MORPHEME_ALIGNED` | The level of conformance of the example with the Leipzig Glossing Rules
[Comment](http://cldf.clld.org/v1.0/terms.rdf#comment) | `string` | 
[Media_IDs](http://cldf.clld.org/v1.0/terms.rdf#mediaReference) | list of `string` (separated by ` `) | References [media.csv::ID](#table-mediacsv)
[Position](http://cldf.clld.org/v1.0/terms.rdf#position) | `integer` | 
`Audio_Start` | `integer` | 
`Audio_End` | `integer` | 
`graid` | list of `string` (separated by `	`) | A morphosyntactic annotation unit with the GRAID scheme (Grammatical relations and animacy in discourse, Haig & Schnell 2014) or ## as clause boundary marker.
`add_orthography` | `string` | The object language text in another orthographical system; in Mandarin or Japanese, for instance, this tier contains the text in its original orthography (hanzi, or kanji and kana) while the utterance tier is a transliteration of the text (pinyin, or romaji).
[Text_ID](http://cldf.clld.org/v1.0/terms.rdf#contributionReference) | `string` | References [texts.csv::ID](#table-textscsv)
`refind` | list of `string` (separated by `	`) | Referent identification with the RefIND scheme (Referent indexing in natural-language discourse, Schiborr et al. 2018). ∅ is used to signal no referent information.
`refindFK` | list of `string` (separated by `	`) | A duplicate refind column is provided, to enable checking referential integrity (via this list-valued foreign key) while still allowing uniform access to the annotation tiers in CLDF SQL. (While the refind column will be converted to a TEXT column in CLDF SQL, this column will be replaced by an association table.)<br>References [referents.csv::refind](#table-referentscsv)
`isnref` | list of `string` (separated by `	`) | The information status of referents with the ISNRef scheme (Information status of new referents, Schiborr et al. 2018: 15), an adaptation of the RefLex scheme (Riester & Baumann 2017). ∅ is used to signal no INNRef annotation.

## <a name="table-textscsv"></a>Table [texts.csv](./texts.csv)

A collection of texts from one language, with shared provenance.

property | value
 --- | ---
[dc:conformsTo](http://purl.org/dc/terms/conformsTo) | [CLDF ContributionTable](http://cldf.clld.org/v1.0/terms.rdf#ContributionTable)
[dc:extent](http://purl.org/dc/terms/extent) | 8


### Columns

Name/Property | Datatype | Description
 --- | --- | --- 
[ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string`<br>Regex: `[a-zA-Z0-9_\-]+` | Primary key
[Name](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | 
[Description](http://cldf.clld.org/v1.0/terms.rdf#description) | `string` | 
[Contributor](http://cldf.clld.org/v1.0/terms.rdf#contributor) | list of `string` (separated by ` and `) | 
[Citation](http://cldf.clld.org/v1.0/terms.rdf#citation) | `string` | 
`Text_Number` | `integer` | Numeric text identifier, used as prefix of referent indices.
[Media_IDs](http://cldf.clld.org/v1.0/terms.rdf#mediaReference) | list of `string` (separated by ` `) | References [media.csv::ID](#table-mediacsv)
`Clause_Count` | `integer` | 
`Speaker` | `string` | 
`Speaker_Gender` | `string`<br>Valid choices:<br> `male` `female` | 
`Speaker_Age` | `integer` | The age of the speaker at the time of recording.
`Speaker_Age_Approximated` | `boolean`<br>Valid choices:<br> `yes` `no` | Whether the age of the speaker was approximated.
`Speaker_Year_Born` | `integer` | The speaker’s year of birth
`Speaker_Year_Born_Approximated` | `boolean`<br>Valid choices:<br> `yes` `no` | Whether the year of birth of the speaker was approximated.
`Type` | `string`<br>Valid choices:<br> `TN` `SN` `AN` | TN = traditional narratives, AN = autobiographical narratives, SN = stimulus-based narratives.
`Year_Recorded` | `integer` | 
`Recording_Length` | `float` | 
[Source](http://cldf.clld.org/v1.0/terms.rdf#source) | list of `string` (separated by `;`) | 

## <a name="table-languagescsv"></a>Table [languages.csv](./languages.csv)

property | value
 --- | ---
[dc:conformsTo](http://purl.org/dc/terms/conformsTo) | [CLDF LanguageTable](http://cldf.clld.org/v1.0/terms.rdf#LanguageTable)
[dc:extent](http://purl.org/dc/terms/extent) | 2


### Columns

Name/Property | Datatype | Description
 --- | --- | --- 
[ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string`<br>Regex: `[a-zA-Z0-9_\-]+` | Primary key
[Name](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | 
[Macroarea](http://cldf.clld.org/v1.0/terms.rdf#macroarea) | `string` | 
[Latitude](http://cldf.clld.org/v1.0/terms.rdf#latitude) | `decimal`<br>&ge; -90<br>&le; 90 | 
[Longitude](http://cldf.clld.org/v1.0/terms.rdf#longitude) | `decimal`<br>&ge; -180<br>&le; 180 | 
[Glottocode](http://cldf.clld.org/v1.0/terms.rdf#glottocode) | `string`<br>Regex: `[a-z0-9]{4}[1-9][0-9]{3}` | 
[ISO639P3code](http://cldf.clld.org/v1.0/terms.rdf#iso639P3code) | `string`<br>Regex: `[a-z]{3}` | 
`Affiliation` | `string` | Genealogical affiliation of the language.
`Areas` | `string` | Areas where the language is spoken.
`Varieties` | `string` | Varieties of the language recorded in this dataset.

## <a name="table-mediacsv"></a>Table [media.csv](./media.csv)

property | value
 --- | ---
[dc:conformsTo](http://purl.org/dc/terms/conformsTo) | [CLDF MediaTable](http://cldf.clld.org/v1.0/terms.rdf#MediaTable)
[dc:extent](http://purl.org/dc/terms/extent) | 42


### Columns

Name/Property | Datatype | Description
 --- | --- | --- 
[ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string`<br>Regex: `[a-zA-Z0-9_\-]+` | Primary key
[Name](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | 
[Description](http://cldf.clld.org/v1.0/terms.rdf#description) | `string` | 
[Media_Type](http://cldf.clld.org/v1.0/terms.rdf#mediaType) | `string`<br>Regex: `[^/]+/.+` | 
[Download_URL](http://cldf.clld.org/v1.0/terms.rdf#downloadUrl) | `anyURI` | 
[Path_In_Zip](http://cldf.clld.org/v1.0/terms.rdf#pathInZip) | `string` | 
`version` | `string` | 
`Size` | `integer` | File size in bytes
`Length` | `float` | Recording length in seconds for audio files.
[Contribution_ID](http://cldf.clld.org/v1.0/terms.rdf#contributionReference) | `string` | References [texts.csv::ID](#table-textscsv)
`Date_Updated` | `date` | 

## <a name="table-referentscsv"></a>Table [referents.csv](./referents.csv)

property | value
 --- | ---
[dc:extent](http://purl.org/dc/terms/extent) | 464


### Columns

Name/Property | Datatype | Description
 --- | --- | --- 
[refind](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | Primary key
[label](http://cldf.clld.org/v1.0/terms.rdf#name) | `string` | 
[description](http://cldf.clld.org/v1.0/terms.rdf#description) | `string` | 
`class` | `string`<br>Valid choices:<br> `hum` `anm` `inm` `bdp` `mss` `loc` `tme` `abs` | The semantic class of the referent; one of hum ‘human’, anm ‘non-human animate’,inm ‘inanimate’, bdp ‘body part’, mss ‘mass’, loc ‘location’, tme ‘time’, or abs ‘abstract’. Only a single label is assigned to a referent, even where a group contains entities belonging to multiple classes. In such cases humans outweigh other animates, animates outweigh inanimates, and inanimates outweigh everything else in no particular order.
[notes](http://cldf.clld.org/v1.0/terms.rdf#comment) | `string` | 

## <a name="table-referentrelationscsv"></a>Table [referent_relations.csv](./referent_relations.csv)

property | value
 --- | ---
[dc:extent](http://purl.org/dc/terms/extent) | 97


### Columns

Name/Property | Datatype | Description
 --- | --- | --- 
[ID](http://cldf.clld.org/v1.0/terms.rdf#id) | `string` | Primary key
`Source_Referent_ID` | `string` | References [referents.csv::refind](#table-referentscsv)
`Target_Referent_ID` | `string` | References [referents.csv::refind](#table-referentscsv)
`Relation` | `string` | The relations of a referent to other referents; including < ‘set member of (partial co-reference)’, > ‘includes (split antecedence)’, and M ‘part-whole’.

