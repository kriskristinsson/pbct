# PointsBet_Backend_Online_Code_Test
This is a simple folder containing a `StringFormatter.cs` file for code enhancement.

For candidates, please follow the below points to complete the test:
- Read the `README.md` file in the root directory, which should be the same file you are reading now. :)
- Go to the `README.md` file
  - Read the comment in the `StringFormatter.cs` file
  - Follow the instructions in the comment to complete the task
- Once complete your solution, please submit the codebase to your GitHub and share the public link with our HR team

Thank you for completing the code test with PointsBet.

---- 

# Feedback from the applicant
## Things done to improve:
* renamed method to ToCommaSeparatedList, ToCommaSepa<u>**t**</u>atedList has a spelling error,
* use string.Join instead of StringBuilder, for performance reasons, string.Join can calculate the final string size immediately and doesn't require resizing, unlike StringBuilder
* moved entry formatting to separate method
* code is now much clearer and concise to read
* I've also addressed couple of logic errors
  1. the original code would throw an exception if the items array is empty; solving this came for free just by using string.Join instead of StringBuilder.
  2. the original code did not take into account input strings that contained the quote character, this is often solved by doubling it (see CSV RFC4180, also T-SQL syntax, et al.)

# Important information for the makers of this code test.
For future reference, be sure to remove your .git folder from the Zip archive before distributing it. 
It revealed the local git repository of this code test which also contains personal information of the person who authored it (by name and work email address)