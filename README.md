# BashCheatSheet

## CSV file
* Count the number of lines: `cat file-name  | wc -l`
* Count the number of columns: `head -n1 file-name | grep -o "," | wc -l` for tab seperated file (.tsv) replace `","` with `" "`.
* Print the first row: `head file-name -n 1`
* Print the first column: `awk -F "\"*,\"*" '{print $1}' file-name`
