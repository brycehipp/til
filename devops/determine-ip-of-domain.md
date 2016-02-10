# Determine The IP Address Of A Domain

The `dig` (domain information grouper) command can be used to get more
information about a domain name. To discover the IP address for a given
domain, invoke `dig` with the domain as an argument.

```bash
$ dig google.com

; <<>> DiG 9.8.3-P1 <<>> google.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 31683
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 0

;; QUESTION SECTION:
;google.com.      IN  A

;; ANSWER SECTION:
google.com.   154 IN  A 216.58.218.206

;; Query time: 29 msec
;; SERVER: 192.168.1.1#53(192.168.1.1)
;; WHEN: Wed Feb 10 14:23:52 2016
;; MSG SIZE  rcvd: 44
```

The *answer section* tells me that the IP address for `google.com` is
`216.58.218.206`.

See `man dig` for more details.
