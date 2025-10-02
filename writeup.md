# Assignment 3 - Write UP

## Description
This assignment completes our movie chatbot system by implementing action functions that query our movie database and building a natural language interface. You implemented functions to search for movies by year, director, and actors, as well as the core search system that matches user queries to appropriate database operations. This builds directly on the pattern matching work from Assignment 2 to create a functional conversational AI system.

## What to complete
1. Complete all action functions in `a3.py` (title_by_year, title_by_year_range, etc.)
2. Implement the `search_pa_list` function to handle pattern matching and responses  
3. Add at least one new movie to the database with proper formatting
4. Create a new pattern/action pair and add it to the pa_list
5. Ensure all provided assert statements pass
6. Complete the reflection questions below
7. Push your code to github for grading

## Reflection Questions

1. What are some key programming concepts or techniques that you learned while completing this assignment?
While completing the assignment, I learned how to pattern match with the inputted data to complete the movie chatbot. A key concept I learned was tuples and how to use them and continued practiced using pattern matching with `_` and `%` to capture variable data inputted from the user. I also learned about NoneType errors and that in this case it was important to always return something so that the code would work...I ran into a few of those at first.


2. How does the overall movie chatbot system work? Explain the flow from when a user types a query to when they receive an answer.
The movie chatbot takes input from the user (well the asserts) in a normal query and processes it by correcting the text and then matching key words. It then goes through pa_list and it finds matches then calls the desired function and searches the `movie_db` for what data is needed. If it finds no results the bot responds with "No answers" and if no pattern matches it returns "I don't understand."


3. What are some real-world applications where this type of pattern-matching chatbot system could be useful? How might you extend or improve this system for practical use?
Some areas where this type of pattern matching could be used is in customer support bots, such as the ones you can find on Chase or Amazon and for Help systems such as IT support for basic problems. The old Siri is also an example as it matched specific patterns to your voice to complete basic actions. To extend it you could add more words for a single thing, synonoms, so that it can support a more variety of phrases.