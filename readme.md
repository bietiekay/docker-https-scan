# HTTPS-Scan Docker image to scan/crawl a given URL for insecure dependencies

A https validation tool based on phantomjs. It can detect more dynamic loaded resources than static HTML analyze. 

## based upon
  - phantomjs
  - https-scan (https://github.com/zordius/https-scan)

## building

 docker build -t https-scan .

## running

 docker run -itd -v $(pwd):/data --name https-scan https-scan

## using

 docker exec -it https-scan /bin/bash

 docker exec -it https-scan https-scan --verbose https://www.url.com

 docker exec -it https-scan https-scan --verbose --file file.txt
