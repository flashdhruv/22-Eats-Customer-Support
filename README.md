# 22-Eats-Customer-Support
### Explanation of Project
#### (From Sayo Everden's Project Plan)
In this project, Team 22 will develop an interactive conversational agent for a call center for food delivery service, T22 Eats. First, the agent will identify if a user is existing business partners( restaurant ) , existing customers or future partners. We will focus on the issue with the current orders from the existing customers in this project. After a caller selects the option for the existing customer and issues with the existing option, our conversational agent program will determine if the customer will get a refund or not with the objective of reducing the number of calls the human operators need to take by 20%.  The common issues include missing items, getting wrong items ,quality of items and taking too long to deliver. Then it will determine if the customer gets refunds, explain why you don’t get a refund or connect the customer to the human operator. 

### How To Run & Compile Code
Run the file Chatbot.java in a program such as Eclipse or similar. 

### Class Organization
The main class of Chatbot.java is comprised of a menu with 6 different choices: missing food, late delivery, quality of food, delivery driver, other, and exit. Based on the choice of the customer, the code will print out a helpful response, ask for more clarification, or provide options for the customer all of which may utilize the 5 helper methods found at the bottom of the code. Essentially, the code uses conditional logic that moves its way through a menu based on the customers response.
### A3 Updates
In A3, we would work on the old bot we created and implement new features to it. Moreover, our bot would also have one more topic on the issues the customers might encounter. All the new features would provide the customers with even better experience when they have any issues. On the background of our program, we record the user's inputs to analyze them using named entity recognition and POS(part-of-speech) tagging to improve the conversation. Lastly, we have unit tests to test certain part of the program. With all the visible and invisible features, we could make the conversation more smoothe.

List of change (for the one not having a snippet, we feel like they are actual functions and could not be examples represented by only parts of the program):
1. GUI- when the programming is running, a new window would pop up to let the user start the conversation.
2. NER- Gather user's inputs and identify each word as an object, name, nationality etc.\
Example: (french, NATIONALITY) (refund,O) 
4. POS- POS is also called grammatical tagging. It gathers user's inputs and identify each word as nouns, adjectives etc.\
Example: hi   UH, yes   UH, I   PRP, missing VBG
5. Unit testing- The unit testing is for the developers to test on a small part of the whole program so it is easier to find mistakes and change them. The main idea of ours are testing whether the bot is working if users correctly type in the texts.\
Example: To check if the user's input are valid. If users hit enter with nothing in the textbox the bot would tell the users "Please type something. We can't understand.".

After A3
For the final project, we were told to implement an API from a given list to the pre-existing bot we had worked on in A3.
I chose to attempt to implement the PayPal API. The aim of this API is to allow transactions to occur. There are two new classes that have been added to the program. The main aim of OrderDetails is to receive the order details from the bot. The user inputs what they want, its price. This information is saved via setter methods and then utilised by the paymentSevices class. This can be done via an additional option on the menu. (option 7). 
