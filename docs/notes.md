# Notas

Código:
ssm.put_parameter(
         Name='/my_test/test',
         Value='NEW_STRING',
         Type='String',
         Overwrite=True
       )


✅ Solution: Convert CSV to a Tab-Delimited .txt File
Option 1: Convert Using Terminal (Mac)

Run this command to replace commas with tabs and save it as a .txt file:

awk -F',' 'BEGIN {OFS="\t"} {print $1, $2, $3, $4, $5, $6}' cambios.csv > cambios.txt

Then upload cambios.txt to Amazon.
