
# Dump remote MongoDB 2.6.x database from OS X El Capitan

## 1) Locally install brew
- http://brew.sh/

## 2) Locally install mongodb 2.6
- Search if mongodb is available.

  ```{r, engine='bash', count_lines}
  brew search mongodb
  ```
- Install MongodDB 2.6

  ```{r, engine='bash', count_lines}
  brew install homebrew/versions/mongodb26
  ```
- info: mongodump works even if mongodb is stopped.

## 3) Locally run mongodump
- Run mongodump

  ```{r, engine='bash', count_lines}
  mongodump --host hostname --port port --db databasename -u username -p
  ```
- Enter your password
- Displaying collections from databasename

  ```{r, engine='bash', count_lines}
  cd ./dump/databasename/ && ls -l
  ```
- Done !
