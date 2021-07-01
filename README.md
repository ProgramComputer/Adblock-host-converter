# Pihole Adlist/Blocklist Converter


 https://help.eyeo.com/en/adblockplus/how-to-write-filters for info on Adblock filters and https://man7.org/linux/man-pages/man5/hosts.5.html on hosts file.



The script will parse all lines in the Adblock list format and extract all complete domains/hostnames (non-regex/wildcarded) into a plain-text list under `/filters` directory. 

## How to Use



To run:
```
python3 adlist_converter.py <url>
```

For example:
```
python3 adlist_converter.py "https://raw.githubusercontent.com/uBlockOrigin/uAssets/master/filters/badware.txt"
```

### Notes:

- Some Adblock lists will include benign domains such as youtube[.]com, which the script will not ignore. Scan the parsed blocklist for common domains before uploading. 
