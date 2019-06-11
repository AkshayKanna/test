FSD.W1.2.B

1. grep -o India marks_rand_2000.csv.1 > india.txt 

   wc -l india.txt

2. grep -o Pakistan marks_rand_2000.csv.1 > pakistan.txt

   head -n 100 marks_rand_2000.csv.1 > top100.txt

   grep Pakistan top100.txt > pak.txt

    wc -l pak.txt 

3. head -n 3 india.txt 

4. tail -n 5 pak.txt
   





FSD.W1.2.C


1. git log > commit.txt

   grep Dave commit.txt

   grep Dave commit.txt > dave.txt 

   wc -l dave.txt

2. grep Apr commit.txt > april.txt

   wc -l april.txt 


3. grep 2018 commit.txt > year.txt
    
   wc -l year.txt 


