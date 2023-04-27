[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-c66648af7eb3fe8bc4f294546bfd86ef473780cde1dea487d3c4ff354943c9ae.svg)](https://classroom.github.com/online_ide?assignment_repo_id=10691093&assignment_repo_type=AssignmentRepo)
# Data Science auf deutschen Songtexten

Dies ist das GitHub Repository für das DIS 22 Projekt im Sommersemester 2023.

[KICK OFF SLIDES](https://docs.google.com/presentation/d/1ZCuXBB6UTuU16BaRwoI_s_GueJkL7dn6yA3QMEmVnOE/edit?usp=sharing)

Genius API Token `aCR_2MFW9c27A8yjxOWlsCfqywd5w1KzwBZJMqncj4psGS0pPdcGzIv05TfkrKIG`

Datensatz REPO: https://github.com/Richard-Sieg-TH-Koln/datensatze-default
## Teamprotokoll

Hier werden die Protokolle für den Fortschritt des Projektes gesammelt. Tragt eure Notizen zum Ende der jeweiligen Kalenderwoche ein.,

### KW 15

- GermanSongCorpus (all.csv) um sämtliche Lyrics im Dataset erweitert.
- Dummy Datasets erstellt, minimal gecleaned (Hausarbeiten, Auflistungen von Songs als Lyrics)
- Dummy Dataset an Statistik Teams weitergegeben.

### KW 17

Erneute Daten Bereinigung des Test Datensets nach Feedback vom Statistik Team:
- Je Song sind alle Informationen / Lyrics jetzt in einer Zeile der CSV-Datei (Vorher Zeilenübergreifend)
- Songtitel aus den Lyrics entfernt

Anforderung Datenquelle für möglichts viele deutsche Songtexte:
- Recherche für Datenquelle im Web und App (Bspw. Spotify / Chat GPT)
- Skript für eine API zu Spotify geschrieben
- Skript für eine API zu Chat_GPT geschrieben (Kostenpflichtige Anfragen)
- Erneute Recherche in der Dokumentation zu Spotipy und wie die Suche nach deutschen Künstlern/Alben/Songs möglich ist

Vielversprechenste Datenquelle für deutsche Künstler/Alben/Songs:
- Mit bspw. Beautifulsoup die Informationen von  der folgenden Website extrahieren: https://musicbrainz.org/area/85752fda-13c4-31a3-bee5-0e5cb1f51dad/artists 


### KW 19

- Hier kommt euer aktueller Stand rein...

### KW 21

- Hier kommt euer aktueller Stand rein...

### KW 23

- Hier kommt euer aktueller Stand rein...

### KW 25

- Hier kommt euer aktueller Stand rein...

## Initiales Setup

```
poetry config virtualenvs.in-project true
poetry env use 3.10.10
poetry install
poetry shell
python -m spacy download de_core_news_sm
```

## Linksammlung

### Datensätze

- [Python Paket für Genius Scraping](https://github.com/johnwmillr/LyricsGenius)
- [Google Dataset Search](https://datasetsearch.research.google.com/search?src=0&query=songtexte&docid=L2cvMTFuZmJqNjkwNA%3D%3D)
- [Music Genres Scraper](https://github.com/robbiebarrat/art-DCGAN/blob/master/genre-scraper.py)
- [Spotify API](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-audio-features)
- https://www.kaggle.com/datasets/carlosgdcj/genius-song-lyrics-with-language-information
- [German Song Lyrics Corpus](https://github.com/lauchblatt/GermanSongLyricsCorpus)

### Data Cleaning

- https://cghlewis.com/blog/data_clean_01/

### Data Science auf Songtexten

- [The Pudding Artikel](https://pudding.cool/projects/vocabulary/index.html)
- [NLP and Rap Lyrics](https://towardsdatascience.com/natural-language-processing-and-rap-lyrics-c678e60073fb)
- https://www.kaggle.com/code/offmann/nlp-on-hiphop-lyrics
- https://www.kaggle.com/datasets/rikdifos/rap-lyrics
- https://rohankshir.github.io/2016/02/28/topic-modeling-on-hiphop/

### Datenanalyse

- https://github.com/approximatelabs/sketch
- https://github.com/Kanaries/pygwalker (geht auch in Richtung Visualisierung)
- https://medium.com/epfl-extension-school/advanced-exploratory-data-analysis-eda-with-python-536fa83c578a
- [Pandas for Machine Learning](https://madewithml.com/courses/foundations/pandas/)

### Visualisierung

- https://python.plainenglish.io/interactive-visualizations-with-pandas-seaborn-and-ipywidgets-173e5d7d6a5e
- https://github.com/z3tt/beyond-bar-and-box-plots/blob/main/README.md

### Klassifizierung

- https://julsimon.medium.com/classifying-song-lyrics-with-natural-language-processing-and-automl-1a31b9f717a9
- https://spcman.github.io/getting-to-know-julia/deep-learning/nlp/song-lyrics-project/
- https://willjarrard.com/post/2022-06-29-classifying-songs-with-nlp/
- https://github.com/wejarrard/classifying_songs_with_nlp
- https://towardsdatascience.com/how-we-used-nltk-and-nlp-to-predict-a-songs-genre-from-its-lyrics-54e338ded537

### Textgenerierung

- https://blog.musixmatch.com/generating-rap-lyrics-with-ai-13fb8d33ab5e
- [DeepRapper Paper](https://aclanthology.org/2021.acl-long.6/)
- [Das Paket zu DeepRapper](https://github.com/microsoft/muzic/tree/main/deeprapper)
