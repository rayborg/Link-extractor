# Link-extractor
Extract links from a file

cat filename | grep http | grep -shoP 'http.*?["|]' | cut -d '=' -f2 | sed 's/.$//' | sort | uniq -c | sort -n 