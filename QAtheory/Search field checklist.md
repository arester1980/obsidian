Check-list
# Question to clarify:

- What fields is search work
- Search on Consist Of or on Full
- Is Register depends?
- Max length of search query
- View Relevant / Sorting results
- Are there context?
- What languages support
- Minimal char for query
- Is there hint?
    - how many char should enter for hint displayed?
    - what max hints are showed?

# Feature to test:

- What if search query is overlenght
- What if search query is empty
- Search works on required field
- Search doesn't work on non-require field
- Register?
- Search on Consist Of or / and on Full
- Mistyping
- Mislanguage
- Different Languages
- Symbols
- Emoji
- Has a add spaces on start or/and after
- Empty query / only spaces in query
- Max length query
- change the words order from one field
- change the words order from diff fields

# Algorithm:

- prioritize checks
- Is it work (positive)?
    - on **each required** fields?
    - off **each non-required** fields?
- search in context or all page/tables/chats etc.?
- SQL injection?

# Extra:

- what happen after searching? user is reach his purpose?
- what if nothing is found?
- what if found too much?