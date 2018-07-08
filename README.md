# Migration of www.imetrical.com from Axial servers
On 2018-07-05 I migrated all the data on axial servers
which hosted multiple sites. 

Published to: http://www.imetrical.com/
Published to: http://daniel-lauzon.com/site-www.imetrical.com/

Root domain imetrical.com is redireceted by hover to www.imetrical.com

Using CNAME record on imetrical.com:
```
CNAME www daneroo.github.io

$ dig ted.mirawatt.com

;; ANSWER SECTION:
ted.mirawatt.com.	713	IN	CNAME	daneroo.github.io.
daneroo.github.io.	3413	IN	CNAME	sni.github.map.fastly.net.
sni.github.map.fastly.net. 3413	IN	A	185.199.108.153
sni.github.map.fastly.net. 3413	IN	A	185.199.109.153
sni.github.map.fastly.net. 3413	IN	A	185.199.110.153
sni.github.map.fastly.net. 3413	IN	A	185.199.111.153
```

## History
The imetrical.com site was originally authored in iWeb.
It was eventually published to axial servers.
It is also still being served by an app-engine app, the code for which is in
- https://github.com/daneroo/iMetrical-Website for content and also
- github.com:daneroo/snookr-gcode/green/iMetricalWeb for zip-serving code
and deployed on AppEngine:
- http://imetrical-web-hrd.appspot.com/iMetrical/Home.html aliased to
- http://imetrical-web.appspot.com/iMetrical/Home.html

It also contains wrapped versions of en and fr sites

- http://imetrical-web.appspot.com/fr/




