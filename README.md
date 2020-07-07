# ConfickerDGA
Listing of Conficker A, & B Domains for 2020-01-01 -> 2020-12-31

Created using downatool2.exe from https://net.cs.uni-bonn.de/wg/cs/applications/containing-conficker/

Bash with Wine: (I'm sure there's a cleaner way to do this)
```
for i in $(echo {188..-177} | xargs -I{} -d ' ' date --date={}' days ago' +"%Y%m%d"); do wine ../downatool2.exe ${i} -a | tail -n+12 >> conficker.a.txt; done
```
