The randomization procedure will use this table to keep track of the counts of subjects in the group assignments.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       |            |         |                       |
| extremities |            |         |                       |
| Head/neck   |            |         |                       |
| Size <2cm   |            |         |                       |
| Size 2-4cm  |            |         |                       |
| Size >4cm   |            |         |                       |
| Male        |            |         |                       |
| Female      |            |         |                       |
| BW <10kg    |            |         |                       |
| BW 10-30kg  |            |         |                       |
| BW >30kg    |            |         |                       |

The last column is the absolute value of the difference between the counts in the treatment and control groups. For example, if 3 treatment dogs have neck tumors and 3 control dogs have neck tumors, then the groups are balanced on neck tumors (3 in each group) and gives an absolute difference of |3-3|=0. 

But if 1 treatment dog and 5 control dogs have neck tumors, then the groups are unbalanced on neck tumors and the absolute value of the difference is |1-5|=4. So, the objective of this randomization approach is to minimize the numbers in the last column.

The table starts out with all zeros because you have no subjects yet.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 0          | 0       | 0                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 0          | 0       | 0                     |
| Size <2     | 0          | 0       | 0                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 0          | 0       | 0                     |
| Male        | 0          | 0       | 0                     |
| Female      | 0          | 0       | 0                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 0          | 0       | 0                     |
| BW >30      | 0          | 0       | 0                     |

For the first subject, flip a coin to determine group membership. Suppose that, from the coin flip, you assign subject 1 to the treatment group, and the subject has a neck tumor, size <2cm is male, and weights 15kg. The table would look like this:

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 0          | 0       | 0                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 1          | 0       | 1                     |
| Size <2     | 1          | 0       | 1                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 0          | 0       | 0                     |
| Male        | 1          | 0       | 1                     |
| Female      | 0          | 0       | 0                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 1          | 0       | 1                     |
| BW >30      | 0          | 0       | 0                     |

There are no control dogs yet, so the control column is still all zeros.

To determine group membership for the second subject, you need to find the effect of subject 2 on group balance, so fill out TWO of the tables that already have the first subject (the table directly above). 

One table has subject 2 in the treatment group, and the other table has subject 2 in the control group. 

Suppose that subject 2 has a trunk tumor, size <2 is male, and weights 15kg. 

If you assigned subject 2 to the treatment, the table would look like this:

Table 1.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 1          | 0       | 1                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 1          | 0       | 1                     |
| Size <2     | 2          | 0       | 2                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 0          | 0       | 0                     |
| Male        | 2          | 0       | 2                     |
| Female      | 0          | 0       | 0                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 2          | 0       | 2                     |
| BW >30      | 0          | 0       | 0                     |

If you assigned subject 2 to the control, the table would look like this:

Table 2.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 0          | 1       | 1                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 1          | 0       | 1                     |
| Size <2     | 1          | 1       | 1                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 0          | 0       | 0                     |
| Male        | 1          | 1       | 0                     |
| Female      | 0          | 0       | 0                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 1          | 1       | 0                     |
| BW >30      | 0          | 0       | 0                     |

Notice how by assigning subject 2 to the control group (Table 2) makes the values in the last column smaller than when subject 2 was assigned to the treatment group (Table 1).

Now, calculate the sum of the last column for each table. For the table with subject 2 assigned to the treatment (Table 1), the sum is 8. For the table with subject 2 assigned to the control (Table 2), the sum is 3. 

Because assigning the subject to the control makes the sum in the last column smaller (last column of Table 1 versus last column of Table 2), assigning the subject to the control improves group balance. So, for this example, assign subject 2 to the control group. 

That means that now, Table 2 is the current table. 

Repeat that process for subject 3 using two copies of Table 2 (the one with subject 2 in the control group, because you assigned subject 2 to the control group). Suppose subject 3 has a neck tumor, size >4, is male, and weights 45kg. 

If you assigned subject 3 to the treatment, the old Table 2 would look like this:

Table 3.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 0          | 1       | 1                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 2          | 0       | 2                     |
| Size <2     | 1          | 1       | 0                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 1          | 0       | 1                     |
| Male        | 2          | 1       | 1                     |
| Female      | 0          | 0       | 0                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 1          | 1       | 0                     |
| BW >30      | 1          | 0       | 1                     |

If you assigned subject 3 to the control, the old Table 2 would look like this:

Table 4.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 0          | 1       | 1                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 1          | 1       | 0                     |
| Size <2     | 1          | 1       | 0                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 0          | 1       | 1                     |
| Male        | 1          | 2       | 1                     |
| Female      | 0          | 0       | 0                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 1          | 1       | 0                     |
| BW >30      | 0          | 1       | 1                     |

Now, calculate the sum of the last column for each table. For the table with subject 3 assigned to the treatment (Table 3), the sum is 6. For the table with subject 3 assigned to the control (Table 4), the sum is 4. 

Because assigning subject 3 to the control makes the sum in the last column smaller (last column of Table 3 vs last column of Table 4), assigning the subject to the control improves group balance. So, for this example, assign subject 3 to the control group. 

Now, Table 4 is the current table.

As you continue to enroll subjects, repeat that process.

For subject 4 use two copies of Table 4 (with subject 3 in the control group, because you assigned subject 3 to the control). Suppose subject 4 has a neck tumor, size >4 is female, and weights 45kg. 

If you assigned subject 4 to the treatment, the old Table 4 would look like this:

Table 5.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 0          | 1       | 1                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 2          | 1       | 1                     |
| Size <2     | 1          | 1       | 0                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 1          | 1       | 0                     |
| Male        | 1          | 2       | 1                     |
| Female      | 1          | 0       | 1                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 1          | 1       | 0                     |
| BW >30      | 1          | 1       | 0                     |

If you assigned subject 4 to the control, the old Table 4 would look like this:

Table 6.

|             |            |         |                       |
| ----------- | ---------- | ------- | --------------------- |
|             | Treatment  | control | \|treatment-control\| |
| trunk       | 0          | 1       | 1                     |
| extremities | 0          | 0       | 0                     |
| Head/neck   | 1          | 2       | 1                     |
| Size <2     | 1          | 1       | 0                     |
| Size 2-4    | 0          | 0       | 0                     |
| Size >4     | 0          | 2       | 2                     |
| Male        | 1          | 2       | 1                     |
| Female      | 0          | 1       | 1                     |
| BW <10      | 0          | 0       | 0                     |
| BW 10-30    | 1          | 1       | 0                     |
| BW >30      | 0          | 2       | 2                     |

Now, calculate the sum of the last column for each table. For the table with subject 4 assigned to the treatment (Table 5), the sum is 4. For the table with subject 4 assigned to the control (Table 6), the sum is 8. 

Because assigning subject 4 to the treatment makes the sum in the last column smaller (Table 5 versus Table 6), assigning the subject to the treatment group improves group balance. 

So, for this example, assign subject 4 to the treatment group. 

Repeat that process for the rest of the subjects as needed. 

There are a couple of other considerations.

Suppose for a new subject the sum in the last column for the two tables is the same. That is, assigning the new subject to the treatment gives the same sum as the assigning the new subject to the control group. In that case, look for bigger differences in the last columns of the two tables. For example,

|             |                               |                            |
| ----------- | ----------------------------- | -------------------------- |
|             | **If assigned to treatment**  | **If assigned to control** |
|             | \|treatment-control\|         | \|treatment-control\|      |
| trunk       | 2                             | 1                          |
| extremities | 5                             | 1                          |
| Head/neck   | 0                             | 1                          |
| Size <2     | 0                             | 1                          |
| Size 2-4    | 0                             | 1                          |
| Size >4     | 0                             | 1                          |
| Male        | 0                             | 1                          |
| Female      | 0                             | 0                          |
| BW <10      | 0                             | 0                          |
| BW 10-30    | 0                             | 0                          |
| BW >30      | 0                             | 0                          |

Both “last columns” add up to 7. But assigning the new subject to the treatment gives a disparity of 5 for extremities. So, you’ll want to assign the new subject to the control group.  If the last columns are basically the same, just flip a coin for group assignment for that particular subject. 

Finally, of course, statisticians never make things easy. I recommend that you can add a little randomization to this process. In the algorithm I described above, the only random part was randomizing the first subject to treatment or control. The rest of the subjects were assigned to groups deterministically. There is nothing wrong with that. However, you can add randomization for each subject by determining their group assignment (as I did above with the algorithm) and then assigning them to that group with 0.8 probability. 

For example, we determined that subject 3, above, should be in the control group. Instead of assigning subject 3 to the control group deterministically, make a “control group hat”: put 10 slips of paper into a hat, with 8 of them labeled “control” and 2 labeled “treatment”. Shake the hat and then draw a slip of paper. It will probably say “control”, and then assign subject 3 to the control group. If the slip of paper says “treatment” then assign subject 3 to the treatment group, even though that isn’t good for balance. 

You will need 2 hats, a control hat with 8 “control” and 2 “treatment”, slips of paper, and a treatment hat with 8 “treatment” and 2 “control” slips of paper.  That way, if you determine that a subject should go in the treatment group, you can use the treatment hat to add a little randomization. If you determine that a subject should go in the control group, you can use the control hat to add a little randomization.

I hope this helps! If something is confusing let me know. I’ve read this over a few times and keep catching mistakes, so I hope you don’t get stuck at a mistake!

 
