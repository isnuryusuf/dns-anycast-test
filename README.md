# dns-anycast-test

- Test via DNS Server in Indonesia
```
for i in `cat list-dns-sort.txt` ; do echo "### QUERY USING DNS $i #####" ; time dig +time=2 +tries=1 knottest1.co.id @$i +noadditional +noquestion +nocomments +nocmd +nostats +short ; echo " " ; done
```

- Test via DNS Server outside Indonesia
```
for i in `cat list-dns-sort-out.txt` ; do echo "### QUERY USING DNS $i #####" ; time dig +time=2 +tries=1 knottest1.co.id @$i +noadditional +noquestion +nocomments +nocmd +nostats +short ; echo " " ; done
```
list: https://public-dns.info/nameserver/id.html
