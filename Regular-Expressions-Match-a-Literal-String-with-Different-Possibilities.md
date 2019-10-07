
# Description

Using regexes like /coding/, you can look for the pattern "coding"in another string.

This is powerful to search single strings, but it's limited to only one pattern. You can search for multiple patterns using the alternationor ORoperator: |.

This operator matches patterns either before or after it. For example, if you wanted to match "yes"or "no", the regex you want is /yes|no/.

You can also search for more than just two patterns. You can do this by adding more patterns with more ORoperators separating them, like /yes|no|maybe/.


# Instruction

Complete the regex petRegexto match the pets "dog", "cat", "bird", or "fish".

# Test
Your regex petRegexshould return truefor the string "John has a pet dog."
Your regex petRegexshould return falsefor the string "Emma has a pet rock."
Your regex petRegexshould return truefor the string "Emma has a pet bird."
Your regex petRegexshould return truefor the string "Liz has a pet cat."
Your regex petRegexshould return falsefor the string "Kara has a pet dolphin."
Your regex petRegexshould return truefor the string "Alice has a pet fish."
Your regex petRegexshould return falsefor the string "Jimmy has a pet computer."

# Challenge Seed
let petString = "James has a pet cat.";

let petRegex = /change/; // Change this line

let result = petRegex.test(petString);


# Solution

let petString = "James has a pet cat.";

let petRegex = /dog|cat|bird|fish/; // Change this line

let result = petRegex.test(petString);
