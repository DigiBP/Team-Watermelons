# Team-Watermelons 🍉

| Team Member                           | E-mail address                                   |
| --------------------------------------| ------------------------------------------------ |
| Edgard Antonio Mourão Junior          | <edgardantonio.mouraojunior@students.fhnw.ch>    |
| Lavina Luke                           | <lavina.luke@students.fhnw.ch>                   |
| Sabrina Cassata                       | <sabrina.cassata@students.fhnw.ch>               |

Supervisor: Maja Spahic


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

### Issues with the current process
The process is completely manual and doesn't take advantage of automation and digitalization. This is not ideal because
* it is **time consuming** and it might require more time to complete than an automated process. Hence, it can slow down the productivity and increase the risk of errors. 
* it is **error-prone** as human processes lead inevitably to mistakes, inaccuracies, and inconsistencies in the work.
* it is **cost intensive** in the long run. 
* it **limits scalability** once helpica.ch needs to accommodate an increased volume. 
* there is **no structured and systematic recording** of requests which can potentially lead to inconsistencies in the work and make it difficult to identify and correct errors.
* it is **difficult to track and monitor** requests which can make it challenging to identify and address issues in a timely manner.

## To-Be feedback system
Automation and digitalization should be employed to improve the To-Be process.

A feedback form will be implemented on the webpage and app of helpica.ch. The form is created with Google Forms.

The process starts with a feedback form beeing sent to the helpica.ch team. First thing, an automation will create **a case number** and acknowledge the receipt of the form to the sender. 

Based on a decision table the system will decide how to continue with the request.

A **complaint** will automatically be forwarded to the 1st level support who will manually asses if the request is complete and can be taken over for resolving. In case information is missing, the sender will be contacted for further information.  

Any **comments** and **questions** submitted will be subject to a sentiment analysis which in case of negative sentiment will trigger an escalation to the CEO. Any neutral or positive comment will be automatically forwarded to the 1st level support for assessment and in case information is missing, the sender will be contacted for further information.  

Any **reporting of a bug** will result in the request being forwarded to the engineering team who will assess it manually. Also in this case if information is missing, the sender will be contacted for further information.

All **requests / suggestions for new features** will be first subject to a sentiment analysis. Should a negative sentiment be detected it will trigger an escalation to the CEO. If the sentiment analysis is neutral or positive, it will be forwarded to the product owner for a manual assessment. If additional information is needed, the sender will be contacted.

**Investigations for payments** will be forwarded to the accounting department. Also in this case if information is missing, the sender will be contacted for further information.

![BPMN_Helpica_As_Is](https://github.com/DigiBP/Team-Watermelons/blob/fa64c26c09ae170aa58dba609cbaa1b72eae6344/BPMN_Helpica_To_Be_V1.png)
