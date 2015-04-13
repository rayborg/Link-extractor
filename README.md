# Link-extractor
Extract links from a file
cat filename | grep http | grep -shoP 'http.*?["|]' | sort | uniq -c | sort -n > urls.txt