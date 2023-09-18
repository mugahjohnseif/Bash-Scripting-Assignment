# Bash-Scripting-Assignment
### Word Count (wc-m and wc -w)
mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/alkanes$ `wc -w -m *.pdb`

|156 |1159 |cubane.pdb|
|--- |   --- |   ----|
|  84|  623| ethane.pdb|
 | 57 | 423| methane.pdb|
| 246| 1829| octane.pdb|
| 165| 1227| pentane.pdb|
| 111|  826| propane.pdb|
| 819| 6087 |total|

mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/alkanes$ `wc -m -w *.pdb >> lengthsF.txt`

mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/alkanes$ `cat lengthsF.txt`

|21| cubane.pdb|-
|---|---|---
 | 13|ethane.pdb|
 | 10| methane.pdb
 | 31 |octane.pdb
 | 22| pentane.pdb
  |16| propane.pdb
 |113| total
| 156| 1159 |cubane.pdb|
 | 84 | 623| ethane.pdb|
 | 57 | 423| methane.pdb|
| 246| 1829 |octane.pdb"|
| 165| 1227| pentane.pdb|
| 111 | 826| propane.pdb|
| 819| 6087| total|

### SORT
mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/alkanes$ `sort -r lengthsF.txt`

|819| 6087 |total
|---|---|---|
| 246 |1829 |octane.pdb
 |165| 1227 |pentane.pdb
 |156 |1159| cubane.pdb
 |113| total
 |111 | 826| propane.pdb
 | 84  |623| ethane.pdb
 | 57 | 423 |methane.pdb
  |31 |octane.pdb
 | 22| pentane.pdb
  |16| propane.pdb
 | 13| ethane.pdb
 | 10| methane.pdb

 ### PIPE FUNCTION

 mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/alkanes$ `wc -l *.pdb | sort -n | head -3 > my_SortedOut.txt`

 mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/alkanes$ `cat my_SortedOut.txt`
 
|10| methane.pdb|
|---|---|
 | 13| ethane.pdb|
 | 16 |propane.pdb|

 ### CUT

 
mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data$ `cd animals-count`

 mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/animals-count$ `ls`

mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/animals-count$ `cat animals.csv`

|2012-11-05,deer,5|
|-------|
|2012-11-05,rabbit,22|
|2012-11-05,raccoon,7|
|2012-11-06,rabbit,19|
|2012-11-06,deer,2|
|2012-11-06,fox,4|
|2012-11-07,rabbit,16|
|2012-11-07,bear,1|

 mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/animals-count$ `cut -d "," -f 2 animals.csv`
 
|deer|
|----|
|rabbit|
|raccoon|
|rabbit|
|deer|
|fox|
|rabbit|
|bear|
 
### LOOPS


 mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/creatures$ `ls`

basilisk.dat  minotaur.dat  unicorn.dat

mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/creatures$ `for a in 1 2 3 4 5 6 7 8 9 10`

> `do`

>  `if a is equal to 5 continue the loop`

> `if [ $a == 5 ]`

> `then`

> `continue`

> `fi`

> `Print the value`
 
> `echo "Iteration no $a"`

> `done`

|Iteration no 1|
|-----|
|Iteration no 2|
|Iteration no 3|
|Iteration no 4|
|Iteration no 6|
|Iteration no 7|
|Iteration no 8|
|Iteration no 9|
|Iteration no 10|


mugah23@CG-LA2-RE13:~/Shell-lesson-data/exercise-data/creatures$ `for i in {0..9}`

> `do`

> `echo $i`

> `done`

|0|
|---|
|1|
|2|
|3|
|4|
|5|
|6|
|7|
|8|
|9|



 

 
