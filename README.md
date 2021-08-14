## Session 14 Assignment
For this project we have 4 files containing information about persons.

### The files are:

personal_info.csv - personal information such as name, gender, etc. (one row per person)
vehicles.csv - what vehicle people own (one row per person)
employment.csv - where a person is employed (one row per person)
update_status.csv - when the person's data was created and last updated
Each file contains a key, SSN, which uniquely identifies a person.

### The assignment has 4 goals:

#### Goal 1
Your first task is to create iterators for each of the four files that contained cleaned up data, of the correct type (e.g. string, int, date, etc), and represented by a named tuple.
For now these four iterators are just separate, independent iterators.

#### Goal 2
Create a single iterable that combines all the columns from all the iterators.
The iterable should yield named tuples containing all the columns. Make sure that the SSN's across the files match!
All the files are guaranteed to be in SSN sort order, and every SSN is unique, and every SSN appears in every file.
Make sure the SSN is not repeated 4 times - one time per row is enough!

#### Goal 3
Next, you want to identify any stale records, where stale simply means the record has not been updated since 3/1/2017 (e.g. last update date < 3/1/2017). Create an iterator that only contains current records (i.e. not stale) based on the last_updated field from the status_update file.

#### Goal 4
Find the largest group of car makes for each gender.
Possibly more than one such group per gender exists (equal sizes).

#### The link to notebook is :
https://github.com/BalajiAJ/EPAi3Session14/blob/main/session14notebook.ipynb
