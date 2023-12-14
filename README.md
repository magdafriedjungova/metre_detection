# Automatic Poetic Metre Detection
A source code repository to the article: "Automatic Poetic Metre Detection" by Kristýna Klesnilová, Karel Klouda, and Magda Friedjungová (_TBA_).

If you find this repository useful, please cite above mentioned article.

## Contents
- `resources`: Resources used inside the implementation
  - `corpusCzechVerse`: Corpus of Czech Verse Git repository
  - `emnlp2017-bilstm-cnn-crf`: BiLSTM-CRF Git repository
- `src`: Implementation
- `requirements.txt`: Python packages installation file
- `.env`: Environment variables file

## Environment for running all jupyter notebooks inside the implementation part
1. Save absolute path of this directory to `WORKING_DIR` environment variable inside `.env` file (create `.env` if not exists): `echo "WORKING_DIR=/absolute/path/to/this/dir" > .env`
2. Create Python3 virtual environment: `python3 -m venv venv`
3. Activate virtual environment: `source venv/bin/activate`
4. Install required packages: `pip3 install -r requirements.txt`

### When using this code as Git repository cloned from [GitHub](https://github.com/friedmag/automatic_poetic_metre_detection.git)
5. Initialize Git submodules located inside `resources`: `git submodule init & git submodule update`

### When using this repository as regular non-Git folder
5. Create directory `resources`: `mkdir resources`
6. Change directory to `resources`: `cd resources`
7. Clone respected Git directories:
      - `git clone git@github.com:magdafriedjungova/emnlp2017-bilstm-cnn-crf.git`
      - `git clone git@github.com:versotym/corpusCzechVerse.git`
