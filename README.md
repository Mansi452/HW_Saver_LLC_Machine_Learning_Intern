# HW_Saver_LLC_Machine_Learning_Intern

### Goal of the Assessment:
To separate out the technical skills from the Raw_Skills_Dataset.csv based on the words and patterns in Example_Technical_Skills.csv.

### Assumptions:
1. Whenever we come across any new skill, we would update it in the Example_Technical_Skills.csv dataset.

### Approach:
1. I start by reading the csv files and applying pre-processing on them.
2. Then I took the intersection of both the lists and find the technical skills in the Raw Skills dataset based on the Example Technical Skills. 
3. And finally stored it in 'HardSkills.txt' file. It contains of all the technical skills and its combination. There are a total of 1116 skill combination. 

### Procedure:
1. First, I read both the csv files through csv library.
2. I read all the rows in the csv, converted it into lower case, strippped all the blank spaces and appended it to a list and later converted it into a set.
3. I started to create a list from Example_Technical_Skills.csv first. 
4. Next, I converted the Raw Skill dataset into a list as well and take the interscetion with list of Example_Technical_Skills.
5. The common skills are appened into another list called tempList1.
6. I proceed with pre-processing on the elements of tempList1 where I first put a filter for mail ids and then replace ',' and '/' with new line and store it in a new list called tempList2.
7. I store the lines from this list into 'HardSkills.txt' so as to get proper elements separated by new lines.
8. I read from the text file again and convert it into a set. This is the finalSet which contains the important skills from the Raw Skills Dataset. 
9. I later re-write the 'HardSkills.txt' file with the finalSet elements which contains a total of 1116 skills. 
