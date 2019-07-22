# dns-anycast-test
```
for i in `cat list-dns-sort.txt` ; do echo "$i ####" ; dig +time=2 +tries=1 knottest1.co.id @$i +short ; done
```
