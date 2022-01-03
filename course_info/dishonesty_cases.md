# Academic Dishonesty Cases

The following stories are real cases of academic dishonesty that we have encountered in classes. 
They are being described here so that it is clear to each of the students what is allowed in this classe. 
In all cases of academic dishonesty, the instructor will file an 
[Academic Dishonesty Report](https://msu.edu/unit/ombud/academic-integrity/academic_dishonesty_report.html) 
and usually fail or severly reduce the student's grade. 

* A student found a solution written by another student (who took the class in a previous year). 
  That student modified the solution (changed variable names, restructured code) and submitted the assignment.
* A student worked closely with another student on an assignment and they showed each other their code in the computer labs. 
  Although no files were exchanged, nor was there any copy/pasting, 
  their solutions converged enough to be detected by my plagiarism detection software.
* A student found a solution to a similar problem in the class written by a third-party 
  (someone not associated with the class). The student submitted a solution based on the found solution, 
  without attribution to the original source.
  
## Attribution 
You must provide attribution if you make use of sources beyond the material given to you in this class. 
The attribution should be commented in your code and/or added to a README file included with your assignment. 
Please ask if you are uncertain as to if a source is allowed to be used in your assignment.

Example project solution with attribution:
```python
# The assignment is to read in a string that looks like "010 001 0101"
# and print out sum of the binary numbers with zero padding.

input_str = input()
bin_strs = input_str.split()


def convert_bin_str_to_int(bin_str):
    # Discovered int function from:
    # http://stackoverflow.com/questions/8928240/convert-base-2-binary-number-string-to-int
    return int(bin_str, 2)


# In discussion with Grant King, we found that the map function
# would be useful in convert both numbers
ints = map(convert_bin_str_to_int, bin_strs)

# This source helped me determine how to print binary numbers with padding:
# http://stackoverflow.com/questions/13599638/how-to-return-a-number-as-a-binary-string-with-a-set-number-of-bits-in-python
print("{0:06b}".format(sum(ints)))
```

Sources which don't require attribution:

* Class-related materials (lectures, example code).
* Documentation from the linked reference websites (python.org, cppreference.com, cplusplus.com).

Everything else, including conceptual discussions with other students should be attibuted.
