
# Team-Watermelons 🍉🍉🍉 

| Team Member                           | E-mail address                                   |
| --------------------------------------| ------------------------------------------------ |
| Edgard Antonio Mourão Junior          | <edgardantonio.mouraojunior@students.fhnw.ch>    |
| Lavina Luke                           | <lavina.luke@students.fhnw.ch>                   |
| Sabrina Cassata                       | <sabrina.cassata@students.fhnw.ch>               |

Supervisor: Maja Spahic


# About helpica.ch ℹ️ 
Helpica.ch is a start-up which aims to position itself as Switzerland’s leading cross-generational multi-sided platform that brings together people who cannot perform daily tasks on their own and seek for Helpies. Helpies are individuals (with a kind heart) who want to offer their support. This can be from simple routine tasks like grocery shopping to more challenging tasks like assembling furniture. Helpica.ch wants to create a network of verified Helpies to create a serving landscape where caregivers can find a trusted Helpie to support a beloved one at one finger click.

![helpica](https://github.com/DigiBP/Team-Watermelons/assets/127504668/08933a63-031f-4c4e-9f80-953ab6d94be4)

# Case: Feedback system for helpica.ch ℹ️ 
The aim of the feedack system is to offer the opportunity to both caregivers and Helpies to communicate with the support-team of helpica.ch for the following categories:
1. General Comments on helpica.ch and its app
2. Ask questions
3. Report a bug about the app
4. Request / suggest a feature that is currently not available
5. Place a complaint
6. Request an investigation for a payment issue

Helpica.ch strives to digitalize its supporting processes. With their innovative business idea, they focus on delivering and developing a user-friendly App. Nevertheless, for the founder of Helpica and his team, it is essential that also processes around the app; In this case, the feedback-management process is efficient, and paint points of today's as-is process are eliminated. 

# Current As-Is Process 🔍 
The following figure, shows the current feedback-management process of Helpica.

![BPMN_Helpica_As_Is_FINAL](https://github.com/DigiBP/Team-Watermelons/assets/127504668/ea249a22-046d-4739-b7b8-0b99ae4716fc)

The current Feedback management process of Helpica contains many user tasks. If a Helpie or Caregiver (in the following referred to “Customers”) want to make a request (e.g. give general feedback, make a feature request, make a complaint etc.) they have to search for the contact data of Helpica and write an e-mail.  

The Customer sends an e-mail, which Helpica receives. The handling feedbacks/requests lies within the responsibility of the 1st Level support. The First Level Support accesses the request. It is checked if all needed information are available. If all information are available ,the 1st Level Support tries to solve the issue. If the final solution can be provided by the 1st Level, a response is send to the requester. If it is not possible to solve the issue, the request is sent to the 2nd Level Support.

The request is assessed by the second Level support. If the 2nd Level Support can solve the issue, the issue is solved. If it is not possible to solve the request, it is escalated to the CEO. The CEO then solves the issue. The response of a solved Issue is send to the customer by the 1st Level support.

## Pain points - Issues with the current process 😕
The process is completely manual and doesn't take advantage of automation and digitalization. This is not ideal from the perspective of Helpica because..
* it is **time consuming** and it might require more time to complete than an automated process. Hence, it can slow down the productivity and increase the risk of errors. 
* it is **error-prone** as human processes lead inevitably to mistakes, inaccuracies, and inconsistencies in the work.
* it is **cost intensive** in the long run. 
* it **limits scalability** once helpica.ch needs to accommodate an increased volume. 
* there is **no structured and systematic recording** of requests which can potentially lead to inconsistencies in the work and make it difficult to identify and correct errors.
* it is **difficult to track and monitor** requests which can make it challenging to identify and address issues in a timely manner.

Further, from a customer's perspective, the process is not ideal because...
* The customer does **not receive any confirmation** of receiving the request
* **long reposonse time**. The customers might become impatient and feeling helpless when clarification is needed



# To-Be-process feedback system ❇️

A to-be-process is created to tackle the pain point of helpica and its customers. With the integration of automation and digitalization, the feedback management process should be improved and relieve the pain points.

**Highlevel overview of process optimisations**
-	Feedback/Request Form
-	Automated case-Number generation & acknowledgement of receipt
-	Sentiment analysis of Feedback/request
-	Case distribution to the correct department based on a decision table
-	Standardized process for the case, that additional information are needed
-	Automated Timer with defined time period – when a ticket is closed automatically
-	Former closing of a case
-	Centralized and structured collection of all data

The following figure shows the created To-Be process:
![BPMN_Helpica_To_Be_FINAL](https://github.com/DigiBP/Team-Watermelons/assets/127504668/07b8fc92-40e2-4ae1-9750-f0af882098c1)

**Description of the To-Be Process**
- To contact Helpica, a feedback form is implemented in Google Forms. With this, a standardized way to already, have structured data, right before the process is kicked of, is ensured.  Depending on the Feedback-Type, the required data fields appear (forms includes conditions). The customers are guided through the form.
- As soon as the form is filled and send out, an automated process creates **a unique case number** and confirmation mail with the case-number is send immediately to the requester.
- In a next step, Sentiment analysis is performed to identify the sentiment of the request
- The feedback is then distributed to the correct department, considering "Feedback Type" and "Sentiment".
<img src="https://github.com/DigiBP/Team-Watermelons/assets/127504668/45df5491-9030-437c-b364-cf1f73b8dde8" width="320">

<img src="https://github.com/DigiBP/Team-Watermelons/assets/127504668/cbd456c6-2259-49f6-998c-f90fdebaaff0" width="820">

- The corresponding department receives the task with all Case-Details. The case is then solved (assessing, checking internal systems etc.)
  - If no additional information is needed to solve the task, the customer is informed about the solution, and the ticket is closed. 
  - If additional information is needed, the customer is being asked for the required information. In this case, an automated Mail is sent to the customer. If a response is received within two days, the task is distributed to the corresponding department again; if not, the customer is informed that the ticket will be closed.

## Benefits of the To-Be Process 💪🏼😄
The process is automated and digitalized and many pains are relived and gains created: 
-	The usage of form allows **storing structured data** at the very beginning of the process
-	An **automated Case-ID** helps to facilitate the overview of all cases for helpica
-	**Automated confirmation** of the request receipt eliminates uncertainties of customers who are wondering if their request has reached helpica.
-	The performed **sentiment analysis support prioritizing** requests
-	**Time savings** for Helpica, since requests are allocated to the department and a standardized process is followed across all departments
-	**Quicker Handling** of the requests. Customers are replied much faster
-	**Structured data**: all the data is collected in a structured form


## Make Scenario 1: Pre-process task
In MAKE an automated pre-process task is creating **a case number**. <br>
<br>
The case number is created by the means of random formula preceeded by the number of the current year to ensure that no duplication happens. <br>
<br>
![Business key creation](https://github.com/DigiBP/Team-Watermelons/assets/127488344/ccf36889-f4e8-4c47-bdb2-2ce8af5e9a17)<br>
<br>
Once the **case number** is created an automated e-mail will be sent to the requester to acknowledge the request stating the **case number**.<br>
<br>
![Feedback received](https://github.com/DigiBP/Team-Watermelons/assets/127488344/73a225b4-698c-4cdb-90f1-ef3bb0200e22)<br>

## Make Scenario 2: Sentiment analysis 
Neutral to make sure that a value is always send back to Camunda (in case it can't recognize at all)
![3_MAKE_Sentiment Analysis](https://github.com/DigiBP/Team-Watermelons/assets/127488344/c46fb93b-01c9-476f-812e-0896f6bbdee4)
![6_MAKE_Sentiment analyis details](https://github.com/DigiBP/Team-Watermelons/assets/127488344/fde87670-ed3c-4e96-acc8-27d22d4adeb6)


## Camunda workflow 1: request distribution and first assessment of the request

**notable limitations of Camunda 7**
Camunda 7, does not support conditions.  The integrated form into the task, could benefit from conditions regarding usability. An option would be to put forms in each user task directly. But since changes must be added to each user task individually, it is highly error-prone. Therefore the team decided to have a general form

## Make Scenario 3: First feedback to customer
![4_Additiona Feedback Reply Customer](https://github.com/DigiBP/Team-Watermelons/assets/127488344/2fb68b57-8d4c-4d2f-a0a5-382f5d1638ea)

## Camunda Workflow 2: 

## Make Scenario 4: Closing of the request
![5_MAKE_Check inbox for reply](https://github.com/DigiBP/Team-Watermelons/assets/127488344/8c0518da-826d-4bd8-b80d-b63d82e44d17)
![7_MAKE_Parser](https://github.com/DigiBP/Team-Watermelons/assets/127488344/b2690ad0-629e-4098-b3c8-c8ce217059e5)


## Outlook

**Error handling**

During the creation of the to-be processed we saw one important are, where a technical error could occur: While performing the sentiment analysis, depending on the inputs, no sentiment is found (e.g if Customer does only wrtie one word). In that case Eden AI, does not detect any sentiment. 

We catch those cases: If sentiment = 0, the sentiment is set as neutral. This also avoids misunderstandings when the case is handled by an agent, who then wonders why the field is empty and whether there is something wrong with the own tool 😉

Further one possible "Technical error" could occur, due to wrong entered email from the Customer. In this case currentyl the process-flow itself will not be interrupted.
-	but customer satisfaction could suffer if the customer does not receive feedback. Even though if he has initially given wrong data

## Conclusion
[Assessment 1: Scenario is innovative and user experience is addressed 10%]
[Assessment 2: Processes are standard compliant and are reflecting conventions. Implementations realise the business processes and workflows are running 10%] <br>
[Assessment 3: Human-centric interfaces are provided. Human tasks are managed.10%]<br>
[Assessment 4: Service integration is running and orchestration is appropriate. Innovative service automation and/or iSaaS implementation. 10%]<br>
[Assessment 5: Appropriate, adequate, and innovative inclusion of automated decision making. 10%]<br>
[Assessment 6: apropriate data model and structured data available. 10%]<br>
[Assessment 7: logical structure and clarity of documentation. Graphical appearance of documentation. 10%]<br>
[Assessment 8: Artefacts are good quality and self-explanatory. Deployment and instantiation are running and available. Instantiation, solution and results are reproducible. 10%]<br>
