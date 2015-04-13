# Link-extractor
Extract links from a file
cat filename | grep http | grep -shoP 'http.*?["|]' | sed s/.$// | sort | uniq -c | sort -n