
# Dump remote MongoDB 2.6.x from local OS X El Capitan

## 1) install brew
- http://brew.sh/

## 2) install mongodb 2.6
- brew search mongodb
- brew install homebrew/versions/mongodb26
- info: mongodump works even if mongodb is stopped.

## 3) run mongodump
- mongodump --host host --port port --db database -u username -p
- cd ./dump/database/
- done !
