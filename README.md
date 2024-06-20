# PolMinePyHesse

Dieses Repository enthält den Code und die Datensätze, die im Rahmen meiner Masterarbeit entstehen. Ich habe auf der Grundlage der semi-strukturierten Rohdokumente
ein XML-TEI-Korpus der Plenarprotokolle der 20. Legislaturperiode des hessischen Landtags generiert.

Auf Grundlage dieses Korpus wird ein Topic Model berechnet. 

## Ordnerstruktur

Die folgende Struktur zeigt die Organisation der Projektordner und -dateien:

```plaintext
PolMinePyHesse/
│ 
├── data/
│   ├── xml
│   ├── xml-tei
│   └── processed_corpus
├── data_outputs/
│   ├── stoppwords.txt -- Ein eigens - mithilfe von tf-idf - generierte Stoppwortliste für das Korpus.
│   ├── tf-idf_results.txt -- Die mittleren tf-idf-Werte.
│   └── ...
├── XSD
│   └── hesseparl_tei.xsd -- Ein XSD-Dokument, um die formale Struktur der Dokumente zu validieren.
├── data_analyzer.py -- Die Analyse der rohen und schemalosen XML-Dokumente.
├── xml_parser.py -- Der Parsers.
├── main.py -- Die Parsing-Prozedur
├── patterns.py -- Reguläre Ausdrücke für den Parser.
├── xml_validator.py -- Funktionen für die Validierung der Wohlgeformtheit und nach dem einem XSD.
├── corpus_manager.py -- Enthält die Klasse CorpusManager, um das tei-Korpus einzulesen und zu verwalten.
└── text_miner.py -- Enthält Funktionen für das Text-Mining.
