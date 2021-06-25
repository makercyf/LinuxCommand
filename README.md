# LinuxCommand

C++ Compile
```
g++ -o test test.cpp
chmod +x test
./test
```

Zip file
```
tar -cvf hello.tar hello/
```

Unzip file
```
tar -xvf hello.tar
```

List files in a directory except some specified extensions
```
ls -I "*.txt" -I "*.pdf"
```

List files in a directory except some specified extensions across all the subdirectories
```
ls -I "*.txt" -I "*.pdf" -R
```

Find duplicate lines in a file and count how many time each line was duplicated
```
sort <file> | uniq -c
```

List out all files in folder and subfolder and count
```
ls -R | uniq -c > record.txt
```

Check specific running process
```
ps aux | grep "[process name]"
```

Check machine resources usage
```
ps aux | head -1; ps aux | sort -rnk 4 | head -10
```

Check storage
```
df -h --total
```

ubuntu remove package
```
apt-get purge [package]
apt-get --purge autoremove [package]
```

Remove dulpicated
```
awk '!seen[$0]++'
```

Remove leading spaces
```
awk '{$1=$1};1'
```

Remove empty line
```
awk /./
```

Remove all character before >
```
sed 's/.*>//'
```

Remove all character after >
```
sed 's/>.*//'
```

Remove spaces
```
tr -d '\040'
```

Remove tabs
```
tr -d '\011'
```

Remove carriage returns (One line text)
```
tr -d '\012'
```

Remove newlines
```
tr -d '\015'
```

Remove spaces, tabs, carriage returns and newlines
```
tr -d '\040\011\012\015'
```

Remove tabs, carriage returns and newlines
```
tr -d '\011\012\015'
```

Regex grep URL
```
grep -oP 'URL/[A-Z]{2}[0-9]{4}'
```
Remember add \ as escape character if end with HTMl element such as /h2

Add echo " to the start of every line using vim
```
:%s/^/echo \"/
```

Add echo " >> report.html to the end of every line using vim
```
:%s/$/\" >> report.html
```

`
Last Update: 2021-06-25 14:46:54
`
