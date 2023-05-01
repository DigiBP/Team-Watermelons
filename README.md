# Team-Watermelons 🍉
Team members: Lavina Luke, Edgard Antonio Mourão Junior, Sabrina Cassata <br>
# About helpica.ch ℹ️
Helpica.ch is a start-up which aims to position itself as Switzerland’s leading cross-generational platform that brings together people who cannot perform daily tasks on their own and seek for Helpies with a kind heart that want to offer their support. This can be from simple chores like grocery shopping to more challenging tasks like assembling furniture. Helpica.ch wants to create a network of verified supporters in order to create a serving landscape where caregivers can find a trusted Helpi to support a beloved one at one finger click.
## Feedback system for helpica.ch
The aim of the feedack system is to offer the opportunity to both caregivers and Helpies to communicate with the team of helpica.ch for the following categories:
1. Comment on helpica.ch
2. Ask questions
3. Report a bug about the app
4. Request / suggest a feature that is currently not available
5. Place a complaint
6. Request an investigation for a payment
## As-Is feedback system

![BPMN_Helpica_As_Is](https://user-images.githubusercontent.com/127488344/235164344-0301a355-84f7-4a10-811b-be07f8d98020.png)
## To-Be feedback system
The process starts with a feedback form beeing sent to the helpica.ch team. The form is created with Google Forms. First thing, an automation will create **a case number** and acknowledge the receipt of the form to the sender. 

Based on a decision table the system will decide how to continue with the request.

A **complaint** will automatically be forwarded to the 1st level support who will manually asses if the request is complete and can be taken over for resolving. In case information is missing, the sender will be contacted for further information.  

Any **comments** and **questions** submitted will be subject to a sentiment analysis which in case of negative sentiment will trigger an escalation to the CEO. Any neutral or positive comment will be automatically forwarded to the 1st level support for assessment and in case information is missing, the sender will be contacted for further information.  

Any **reporting of a bug** will result in the request being forwarded to the engineering team who will assess it manually. Also in this case if information is missing, the sender will be contacted for further information.

All **requests / suggestions for new features** will be first subject to a sentiment analysis. Should a negative sentiment be detected it will trigger an escalation to the CEO. If the sentiment analysis is neutral or positive, it will be forwarded to the business development team for a manual assessment. If additional information is needed, the sender will be contacted.

**Investigations for payments** will be forwarded to the accounting department. Also in this case if information is missing, the sender will be contacted for further information.
