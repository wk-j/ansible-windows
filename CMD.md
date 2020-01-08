## Command

```bash
curl --header "Content-Type: application/soap+xml;charset=UTF-8" http://192.168.33.30:5985/wsman \
    --basic  \
    -u vagrant:vagrant \
    --data '<s:Envelope xmlns:s="http://www.w3.org/2003/05/soap-envelope" xmlns:wsmid="http://schemas.dmtf.org/wbem/wsman/identity/1/wsmanidentity.xsd"><s:Header/><s:Body><wsmid:Identify/></s:Body></s:Envelope>'
```

