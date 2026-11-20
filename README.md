# Practice---Boolean-Filtering
# Practice exercise from week 6 NumPy class

import numpy as np

scores = np.array([45, 67, 82, 91, 38, 74, 56, 88, 63, 49])

# Find scores greater than or equal to 70
passed = scores[scores >= 70]
print("passed  scores:", passed)

# Find scores below 50
below_50 = scores[scores < 50]
print("below_50:", below_50)

# Find scores between 60 and 80 inclusive
between_60_and_80 = scores[(scores >= 60) & (scores <= 80)]
print("between_60_and_80:", between_60_and_80 )

# count how many students passed
pass_mark = 50
passed = np.sum(scores >= pass_mark)
print("students who passed:", passed)

# calculate the average of only the passing students
passing_students = scores[(scores >= 50)]
average = np.mean(passing_students)
print("the avearge is:", round(average, 2))





