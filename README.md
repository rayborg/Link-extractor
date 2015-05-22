# Link-extractor
Extract links from a pipe-seperated file:

grep http filename | grep -shoP 'http.*?["|]' | sed s/.$// | sort | uniq -c | sort -n