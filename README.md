# dns-anycast-test

- Test via DNS Server in Indonesia
```
for i in `cat list-dns-sort.txt` ; do echo "$i ####" ; dig +time=2 +tries=1 knottest1.co.id @$i +short ; done
```

- Test via DNS Server outside Indonesia
```
for i in `cat list-dns-sort-out.txt` ; do echo "$i ####" ; dig +time=2 +tries=1 knottest1.co.id @$i +short ; done
```
