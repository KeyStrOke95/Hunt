# Hunt
A repository that contains a list of subdomains for bug bounty hunting (for personal use)

## Extraction
```
grep -o '"fullURL":"[^"]*' sub.json | awk -F '"' '{print $4}' | cut -d ":" -f1,2 > subdomains.json
```
