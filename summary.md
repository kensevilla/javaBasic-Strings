
**should_be_immutable**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> That String.replace will look for the target string and replace it with the specified new string value. https://www.javatpoint.com/java-string-replace

**Why the test failed at first?**

-> Because the variable areSame at first is empty and the two variables have different values.

**Why you corrected the test that way?**

-> Since the originalString is "The original string" and after the replace line the modifiedString will be "The new string" then areSame should be false.

**Do you have further questions on this knowledge point?**

-> None


**all_modification_method_will_create_new_string**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> That String.trim will remove all the white spaces at the front and end of the string.
https://www.geeksforgeeks.org/java-string-trim-method-example/

**Why the test failed at first?**

-> Because the variable areSame at first is empty and the two variables have different values.

**Why you corrected the test that way?**

-> Since the originalString has whitespaces at the end of it, using trim will remove the whitespaces thus making the value of the two variables different.

**Do you have further questions on this knowledge point?**
-> None



**will_create_new_string_when_concat**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> that += will concat the original value of the string to the next string. https://stackoverflow.com/questions/7456462/what-does-the-operator-do-in-java/7456548

**Why the test failed at first?**

-> Because the variable areSame at first is empty and the two variables have different values.

**Why you corrected the test that way?**

-> Since the variable copyOfOriginalString will just have the first value of originalString which is "Part one. " and variable originalString will be changed afterwards by adding value "Part two", then the two variables will have a different value.

**Do you have further questions on this knowledge point?**
-> None




**should_taken_string_apart**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> To remove a certain part of a string. https://www.javatpoint.com/java-string-replace

**Why the test failed at first?**

-> Because there is no logic to change the variable partOfString which is null to be the same with expectedSring which is "is great"

**Why you corrected the test that way?**

-> Since the expectedString is "is great" and the originalString is "Java is great" then we can simply replace "Java " with a blank space so the two variables will have the same values.

**Do you have further questions on this knowledge point?**

-> None




**should_taken_string_apart_continued**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> To get a specific part of a string. https://stackoverflow.com/questions/3481828/how-to-split-a-string-in-java

**Why the test failed at first?**

-> Because there is no logic that will use the variable originalString to match the value of the expected value which is "is".

**Why you corrected the test that way?**

-> Since the expectedString is "is" and the originalString is "Java is great" then we can just split the originalString to get the expected value.

**Do you have further questions on this knowledge point?**

-> None

**What if the input arguments is out of range of the string?**

-> the test will always fail

**What will happen if the the starting index is greater than the ending index?**

-> an ArrayIndexOutOfBoundsException will be triggered.

 **What will happen if the input string is of null reference?**
 
-> a NullPointerException will be triggered.



**should_break_string_into_words**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> the use of String.split. https://www.geeksforgeeks.org/split-string-java-examples/

**Why the test failed at first?**

-> because there is no logic to change the variable words[] to match the expected result.

**Why you corrected the test that way?**

-> since the variable sentence has the values that will match the expected value, then using will String.split will just convert the string into an array of string

**Do you have further questions on this knowledge point?**

-> None



**should_break_string_into_words_customized**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> the use of String.split. https://www.geeksforgeeks.org/split-string-java-examples/

**Why the test failed at first?**

-> because the variable words[] at first is null and is not matching the expected value.

**Why you corrected the test that way?**

-> since the variable sentence is "This/is/Mike" and expected value is {"This", "is", "Mike"} then we can just split the string into array of string with the use of '/'

**Do you have further questions on this knowledge point?**

-> None



**should_create_ascii_art**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> the use of StringBuilber and append. https://www.geeksforgeeks.org/stringbuilder-class-in-java-with-examples/

**Why the test failed at first?**

-> at first we can see that variable builder has no value which is different from the expected value.
**Why you corrected the test that way?**

-> since the variable is a StringBuilder, I can just use the method append to basically concat the string that I want to add. 

**Do you have further questions on this knowledge point?**

-> None



**should_calculate_checksum_of_a_string**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> that we can simply put a character in an int variable and it will be automatically casted into its ASCII value. https://stackoverflow.com/questions/16458564/convert-character-to-ascii-numeric-value-in-java

**Why the test failed at first?**

-> at first I was trying to convert the character to its alphabetic order but the value is not the same with the expected. 

**Why you corrected the test that way?**

-> since putting a character in an int variable will automatically cast it, I can just loop the string to get the characters and add it.

**Do you have further questions on this knowledge point?**

-> None


**should_convert_unicode_escape**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> that we can use hexadecimal for special characters with the proper use of escape. https://stackoverflow.com/questions/21522770/unicode-escape-syntax-in-java

**Why the test failed at first?**

-> at first I was trying to put the value of the unicode directly without using escape.

**Why you corrected the test that way?**

-> I just need to use '\' to make java think that it is not an actual sting but instead a hexadecimal value for a character

**Do you have further questions on this knowledge point?**

-> None


**should_reverse_a_string**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> the use of String.charAt and for loop. https://beginnersbook.com/2013/12/java-string-charat-method-example/

**Why the test failed at first?**

-> because the variable reversed is set first to null and does not match the expected output.

**Why you corrected the test that way?**

-> since the variable original is just the reversed string of the expected output, then we can just loop the original string and concat the last character to the first character to match the output.

**Do you have further questions on this knowledge point?**



**should_compare_string_with_different_cases**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> the use of String.equalsIgnoreCase. https://beginnersbook.com/2013/12/java-string-equals-and-equalsignorecase-methods-example/
**Why the test failed at first?**

-> because the variables equalResult and equalIgnoreCaseResult are first set to empty.

**Why you corrected the test that way?**

-> since for the variable equalResult, the logic is to just use String.equals then the variables upperCased and lowerCased will not match since they have different case so it will return false.
    however, for the variable equalIgnoreCaseResult, String.equalsIgnoreCase is used which will ignore the case so it will return true.

**Do you have further questions on this knowledge point?**



**should_format_string**

**What is the knowledge point of the test? Where is the official document to the knowledge point?**

-> the use of String.format. https://www.javatpoint.com/java-string-format
**Why the test failed at first?**

-> because the variable text are first set to null.

**Why you corrected the test that way?**

-> since String.format is used then it will just substitute the value with the use of the char %

**Do you have further questions on this knowledge point?**