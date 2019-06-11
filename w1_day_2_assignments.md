# Week 1 - Day 2

**NOTE:** Follow the instructions carefully and follow coding discipline

## FSD.W1.2.A (10 min)

- Go to your home directory `cd ~` and create a folder called `assignments`   
- Create a folder called `week1` inside `assignments` folder  
- Create a folder called `day2` inside `week1` folder  
- Navigate to the folder `assignments/week1/day2` 
- All the work should be in this folder

## FSD.W1.2.B (40 min)

**NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM**

Download the file https://raw.githubusercontent.com/masai-school/assignments-data/master/data/junk/marks_rand_2000.csv

The files contains marks the data of 2000 students from India and Pakistan one for each line in the below format

``` 
23 India 5cf9c9be70765c6c741bd34a
43 Pakistan 5cf9c9be70765c6c741bd352
.
.

```
1. Find the total number of students from India

```
1500
```

Commands on how you got the answer

```
grep -o India marks_rand_2000.csv.1 > india.txt 

wc -l india.txt
```
2. No of students from Pakistan who are in top 100 list based on the marks scored
```
27
```

Commands on how you got the answer

```
sort marks_rand_2000.csv.1 > sort.txt

head -n 100 sort.txt  > top100.txt

grep Pakistan top100.txt > m.txt

wc -l m.txt
```
3. Top 3 students from India based on the marks scored
```
35 India 5cf9c9be70765c6c741bd355
100 India 6cf9c9be70765c6c741bd387
7 India 6cf9c9be70765c6c741bd57b
```

Commands on how you got the answer

```
head -n 3 india.txt

```
4. Bottom 5 students from Pakistan based on the marks scored
```
87 Pakistan 5cf9c9be70765c6c741bd5f2
33 Pakistan 5cf9c9be70765c6c741bd657
45 Pakistan 5cf9c9be70765c6c741bd62a
81 Pakistan 5cf9c9be70765c6c741bd6c8
0 Pakistan 5cf9c9be70765c6c741bd62f
```

Commands on how you got the answer

```
tail -n 5 pak.txt
```

## FSD.W1.2.C (30 min)

**NOTE: SAVE ALL THE COMMANDS ON HOW YOU ARRIVED AT THE ANSWER YOU NEED TO SUBMIT THEM**

Clone the repo https://github.com/dwmkerr/hacker-laws inside `assignments/week1/day2` folder

1. Find the total number of commits done by the user with the name `Dave`

```
91 
```

Commands on how you got the answer

```
 git log > commit.txt

 grep Dave commit.txt

 rep Dave commit.txt > dave.txt 

 wc -l dave.txt
```

2. Find the total no of commits done in the month of April

```
10
```
Commands on how you got the answer

```
grep Apr commit.txt > april.txt

wc -l april.txt 
```

3. Find the total no of commits done in the year 2018

```
33
```
Commands on how you got the answer

```
grep 2018 commit.txt > year.txt
    
wc -l year.txt
```

## FSD.W1.1.D (20 min)

- Clone the repo https://github.com/masai-school/full-stack-dev inside `~/repos` folder
- Navigate to the folder `~/repos/full-stack-dev/`
- Copy the `course/week_1/day_1/w1_day_2_assignments.md` file to the `test` repository which should be at `~/repos/test`
- Open the file `w1_day_2_assignments.md` in the text editor using GUI and fill all the answers
- Sync your `test` repo online with the solutions