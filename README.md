
# Team-Watermelons 🍉🍉🍉 

| Team Member                           | E-mail address                                   |
| --------------------------------------| ------------------------------------------------ |
| Edgard Antonio Mourão Junior          | <edgardantonio.mouraojunior@students.fhnw.ch>    |
| Lavina Luke                           | <lavina.luke@students.fhnw.ch>                   |
| Sabrina Cassata                       | <sabrina.cassata@students.fhnw.ch>               |

Supervisor: Maja Spahic


# About helpica.ch ℹ️ 
helpica.ch is a start-up which aims to position itself as Switzerland’s leading cross-generational multi-sided platform that brings together people who cannot perform daily tasks on their own and seek for Helpies. Helpies are individuals (with a kind heart) who want to offer their support. This can be from simple routine tasks like grocery shopping to more challenging tasks like assembling furniture. helpica.ch wants to create a network of verified Helpies to create a serving landscape where caregivers can find a trusted Helpie to support a beloved one at one finger click.

![helpica](https://github.com/DigiBP/Team-Watermelons/assets/127504668/08933a63-031f-4c4e-9f80-953ab6d94be4)
# Case: Feedback system for helpica.ch ℹ️ 
The aim of the feedack system is to offer the opportunity to both caregivers and Helpies to communicate with the support-team of helpica.ch for the following categories:
1. General Comments on helpica.ch and its app
2. Ask questions
3. Report a bug about the app
4. Request / suggest a feature that is currently not available
5. Place a complaint
6. Request an investigation for a payment issue

helpica.ch strives to digitalize its supporting processes. With their innovative business idea, they focus on delivering and developing a user-friendly App. Nevertheless, for the founder of helpica.ch and his team it is essential that also processes around the app, in this case the feedback-management process, is efficient, and paint points of today's as-is process are eliminated. 

# Current As-Is Process 🔍 
The following figure, shows the current feedback-management process of helpica.ch.

![BPMN_Helpica_As_Is_FINAL](https://github.com/DigiBP/Team-Watermelons/assets/127504668/ea249a22-046d-4739-b7b8-0b99ae4716fc)

The current Feedback management process of helpica.ch contains many user tasks. If a Helpie or Caregiver (in the following referred to “Customers”) want to make a request (e.g. give general feedback, make a feature request, make a complaint etc.) they have to search on helpica.ch for the contact data and write an e-mail or they fill in the contact us form. <br>

<img src="https://github.com/DigiBP/Team-Watermelons/assets/127488344/0b558baa-8eaa-4ee3-82bb-c2b983b1810d" width="520">

helpica.ch then receives an e-mail. The handling feedbacks/requests lies within the responsibility of the 1st Level support. The First Level Support accesses the request. It is checked if all needed information are available. If all information are available ,the 1st Level Support tries to solve the issue. If the final solution can be provided by the 1st Level, a response is send to the requester. If it is not possible to solve the issue, the request is sent to the 2nd Level Support.

The request is assessed by the second Level support. If the 2nd Level Support can solve the issue, the issue is solved. If it is not possible to solve the request, it is escalated to the CEO. The CEO then solves the issue. The response of a solved Issue is send to the customer by the 1st Level support.

## Pain points - Issues with the current process 😕
The process is completely manual and doesn't take advantage of automation and digitalization. This is not ideal from the perspective of helpica.ch because...
* it is **time consuming** and it might require more time to complete than an automated process. Hence, it can slow down the productivity and increase the risk of errors. 
* it is **error-prone** as human processes lead inevitably to mistakes, inaccuracies, and inconsistencies in the work.
* it is **cost intensive** in the long run. 
* it **limits scalability** once helpica.ch needs to accommodate an increased volume. 
* there is **no structured and systematic recording** of requests which can potentially lead to inconsistencies in the work and make it difficult to identify and correct errors.
* it is **difficult to track and monitor** requests which can make it challenging to identify and address issues in a timely manner.

Further, from a customer's perspective, the process is not ideal because...
* The customer does **not receive any confirmation** of having send a request.
* **long reposonse time**. The customers might become impatient and feeling helpless when clarification is needed.

# To-Be-process feedback system ❇️

A to-be-process is created to tackle the pain points of helpica and its customers. With the integration of automation and digitalization, the feedback management process should be improved and relieve the pain points. The to-be process was created based on inputs from Helpica.

**Highlevel overview of process optimisations**
-	Feedback/request form
-	Automated case-number generation & acknowledgement of receipt
-	Sentiment analysis of feedback/request
-	Case distribution to the correct department based on a decision table
-	Standardized process in case that additional information is needed
-	Automated timer with defined time period – after that a ticket is closed automatically
-	Formal closing of a case
-	Centralized and structured collection of all data

The following figure shows the created To-Be process:
<br>

![BPMN_Helpica_To_Be_FINAL](https://github.com/DigiBP/Team-Watermelons/assets/127504668/07b8fc92-40e2-4ae1-9750-f0af882098c1)

**Description of the To-Be Process**
- To contact helpica.ch, a feedback form is implemented in Google Forms. With this, it is ensured that data is collected in a standardized and structured way, event right before the process is kicked of. Depending on the feedback-type, the required data fields appear (forms includes conditions). The customers are guided through the form.

<img src="https://github.com/DigiBP/Team-Watermelons/assets/127488344/9f7dd232-8260-461d-bdb6-2a0e2ffcc197" width="420">
     
- As soon as the form is filled and send out, an automated process creates **a unique case number** and confirmation mail with the case-number is send immediately to the requester.
- In a next step, a **sentiment analysis** is performed to identify the feeling of the request.
- The case/task is then distributed to the correct department, considering "feedback type" and "sentiment". The 

| <img src="https://github.com/DigiBP/Team-Watermelons/assets/127504668/45df5491-9030-437c-b364-cf1f73b8dde8" width="320">                        | <img src="https://github.com/DigiBP/Team-Watermelons/assets/127504668/cbd456c6-2259-49f6-998c-f90fdebaaff0" width="820">                                   |
| --------------------------------------| ------------------------------------------------ |

- The corresponding department receives the task with all case details. The case is then solved (assessing, checking internal systems etc.)
  - If no additional information is needed to solve the task, the customer is informed about the solution, and the ticket is closed. 
  - If additional information is needed, the customer is being asked for further information. In this case, an automated mail is sent to the customer. If a response is received within two days, the task is distributed to the corresponding department again; if not, the customer is informed that the ticket will be closed.
  
 **Remarks - limitations of Camunda**
 - A timer has been integrated to the model after the sentiment analysis to ensure, that the data rows are updated correctly. Further Camunda 7 has some unknown issues,  if a user task is followed after a service task.
 - Based on the input from our expert/coach we switched in the decision table from "Unique" to the hit-policy "First" since Camunda had some issues with it. After implementing this change, we didn't face any longer issues.  

## Benefits of the To-Be Process 💪🏼😄
The process is automated and digitalized and many pains are relived and gains created: 
-	The usage of the form allows **storing structured data** at the very beginning of the process
-	An **automated case-number** helps to facilitate the overview of all cases for helpica.ch
-	**Automated confirmation** of the request receipt eliminates uncertainties of customers who are wondering if their request has reached helpica.ch
-	The performed **sentiment analysis supports prioritizing** requests
-	**Time savings** for helpica.ch, since requests are allocated to the department and a standardized process is followed across all departments
-	**Quicker handling** of the requests. Customers receive replies much faster
-	**Structured data**: all the data is collected in a structured form


## Make Scenario 1: Pre-process task
In MAKE an automated pre-process task is creating **a case number**. 
<br>

Once the **case number** is created an automated e-mail will be sent to the requester to acknowledge the request stating the **case request**.
<br>
| <img src="https://github.com/DigiBP/Team-Watermelons/assets/127504730/e840e012-2537-4608-9cca-522b5d362195" width="520">                        |
| --------------------------------------|

<br>

![Feedback received](https://github.com/DigiBP/Team-Watermelons/assets/127488344/73a225b4-698c-4cdb-90f1-ef3bb0200e22)<br>
<br>
- Google Sheets (Watch New Rows): Check for new entries from the form google sheet
- Tools (Set variable): Create the case number (business key) by the means of random formula with the current year as perfix to ensure that no duplication happens.<br>

<img src="https://github.com/DigiBP/Team-Watermelons/assets/127488344/563679f6-6af1-48c9-85b8-434b2ab28db0" width="420">

- Google Sheets (Update a Row): Update the case number (business key) in the Google Sheets.
- Gmail (Send an email): Send to the requester an acknowledgement email with the case number.
- HTTP (Make a request): Start the process in Camunda and send the following information - name, e-mail, feedback type, customer feedback, phone and case number (business key).


## Make Scenario 2: Sentiment analysis 
This scenario performs the sentiment analysis of the customer's feedback. As a start-up, for Helpica's CEO it is critical to be informed of negative feedback so the issue can be quickly addressed.
<br> 

![3_MAKE_Sentiment Analysis](https://github.com/DigiBP/Team-Watermelons/assets/127488344/c46fb93b-01c9-476f-812e-0896f6bbdee4)<br>
<br>
- HTTP Make a requets: Using "fetchAndLock" get the requets from the service task "identify sentiment".
- Google Sheets (Search Rows): Based on the business key, indentify the row to select the feedback text.
- Eden AI (Identify General Sentiment of a Text): Via API identify the sentiment analysis from the text using IBM as provider.
- Google Sheets (Update a Row): Update the result of the sentiment analysis in the Google Sheets in the row previously identified. If the text is too short and IBM cannot identify the sentiment, a neutral sentiment is saved to ensure a value is always sent back to Camunda.<br>

<img src="https://github.com/DigiBP/Team-Watermelons/assets/127488344/07198659-317e-4998-84cd-ec95e553cf65" width="720">

- HTTP (Make a Request): Send the result of the sentiment analysis to Camunda.

## Camunda workflow 1: request distribution and first assessment of the request<br>
<br>
The request with all information is received in Camunda.
<br>


![Form1](https://github.com/DigiBP/Team-Watermelons/assets/127504730/457a3fb9-06d8-44f6-a831-d006d64ad13e)<br>

-	The task is assigned to the responsible department according to the decision table. The employees of the responsible department find a new entry in the task list, claim the task and can solve it. 
-	The Camunda form shows all data entered by the requester and the output of the sentiment. Based on the sentiment, the employees can easily prioritize. 
-	The responsible department can solve the issue. The agent can choose if additional information is needed:
     - If yes, the corresponding field is filled
     - If no, then final solution/feedback is already given
-	A service task will continue with the workflow

**Notable limitations of Camunda 7**<br>
Camunda 7 does not support conditions. The integrated form in the task could benefit from conditions regarding usability. An option would be to put forms in each user task directly. But since changes must be added to each user task individually, it is highly error-prone. Therefore the team decided to have a general form.

## Make Scenario 3: Reply to customer
This scenario is responsible for sending the reply to the customer. It checks if additional information is needed before sending the e-mail.
<br>
![reply2](https://github.com/DigiBP/Team-Watermelons/assets/127504730/74ae4831-5c42-42e7-96e8-a09f036d618f)<br>
<br>

![4_Additiona Feedback Reply Customer](https://github.com/DigiBP/Team-Watermelons/assets/127488344/2fb68b57-8d4c-4d2f-a0a5-382f5d1638ea)<br>
- HTTP (Make a request): HTTP Make a request: Using "fetchAndLock" get the requets from the service task "ask for additional information".
- Google Sheets (Search Rows): Based on the business key, indentify the row to be updated.
- Google Sheets (Update a Row): Update the row with the "Feedback Needed" ("yes" or "no") and the "reply text".
- Router: Check if the result of the "Feedback Needed" is "yes" or "no" and set the route accordingly.
- Gmail (Send an email): Send the reply to the customer, either the final reply or asking for further information.
- HTTP (Make a request): Send the process back to Camunda.

## Camunda Workflow 2:<br> 

The request is received in camunda.  The task is assigned to the responsible department.

![Form2](https://github.com/DigiBP/Team-Watermelons/assets/127504730/aeba6db3-0a9d-4d8b-9629-0e521632c64d)<br>

-	The Camunda form shows all information including what additional information was asked for and what the reply of the customer is.
-	The responsible department can solve the issue. The agent can choose if additional information is needed:
     -	If yes, the corresponding field is filledo	If yes, the corresponding field is filled
     -	If no, then final solution/feedback is already given
-	A service task will continue with the workflow



## Make Scenario 4: Check additional feedback from customer<br>
Check Helpica's inbox for the customer further information feedback email. There is a rule in gmail to set "Helpica Cases New" label for new emails.<br>

![5_MAKE_Check inbox for reply](https://github.com/DigiBP/Team-Watermelons/assets/127488344/8c0518da-826d-4bd8-b80d-b63d82e44d17)<br>
- Gmail (watch emails): Check for new email in "Helpica Cases New" folder (label) which contains "Case Number" in the subject.
- Gmail (Move an email): Move the email from "Helpica Cases New" to Helpica Cases Archive" based on email's UID.
- Text paser (Match pattern (Advanced)): Select only the case number (business key) from the email's subject.
- Text paser (Match pattern (Advanced)): Split the email body between Helpica reply and customer feedback and select only the customer feedback. (Necessary due Camunda 7 limitaion - "A <Textarea> is not supported by Camunda Platform 7.18")
- Text parser (Replace): Replace from the customer feedback newline (line feed) by space. (Necessary due Camunda 7 limitaion - "A <Textarea> is not supported by Camunda Platform 7.18").<br>
  <br>
![7_MAKE_Parser](https://github.com/DigiBP/Team-Watermelons/assets/127488344/b2690ad0-629e-4098-b3c8-c8ce217059e5)<br>
- Tools (Set variable): Create a variable out of the customer feedback text. Necessary to use in HTTP (Make a request).
- Google Sheets (Search Rows): Indentify the row to be updated based on the business key.
- Google Sheets (Update a Row): Update the last customer feedback into the google sheets.
- HTTP (Make a request): Send the process back to Camunda with the additional feedback from the customer.

# Outlook 👀

All processes can be continuously improved. Possible enhancements for the future are: 
- The already integrated decision table allows the distribution of the requests to the correct department. Helpica starts with the first setup, and according to experience, the allocation to the internal roles/department can be adjusted flexibly.   
- In addition to the available Google form, we will introduce alongside also a chatbot, which asks the questions from the form and can also include suggestions from an FAQ section based on similar cases.
- Error handling: Error handling is an essential aspect of a process. During the design of the To-Bo process, we have included one error handling in make: While performing the sentiment analysis, depending on the inputs, no sentiment is found, e.g. the customer does only write one word). In that case, Eden AI does not detect any sentiment. We catch those cases: If sentiment = null, the sentiment is set to "neutral". Primarily this change had been made to avoid misunderstandings when the case is handled by an Helpica-agent, who then wonders why the field is empty and whether there is something wrong with the own tool 😉
  Further possible enhancement regarding technical error handling can be included for service tasks. For the Service Task "ask additional information," an E-Mail is sent to the requester. If the requester entered the wrong e-mail address or the requester's mailbox is full, the E-Mail does not reach the requester. In this case, currently, the process flow is not interrupted. After two days with no reply, the case will be closed. But to increase customer satisfaction, it can be evaluated if a user task should be integrated to catch such an error. The following shows a possible implementation:
<img src="https://github.com/DigiBP/Team-Watermelons/assets/127504668/628cb64e-9d23-49d6-a9c2-c1d35af4f5f8" width="400">

# Conclusion 🔚

In conclusion we would like to highlight our journey, challenges faced, and collaborative efforts that led to successful outcomes.
By working on the digitalization of the feedback process we are able to create and share valuable inputs for helpica.ch. Our solution helps in eliminating several pain points and enhances the overall workflow. 

One of the most underestimated aspects we encountered during the project was the configurations in MAKE. With a high workload and numerous lessons learned, we soon realized the significance of understanding the complexities involved. One of the biggest challenges we faced was the parser in MAKE, where we initially lacked knowledge of certain small tricks that proved crucial for efficient implementation.

However, our greatest achievement was finding a solution to incorporate the sentiment analysis with MAKE. This task was far from easy, because there are several providers that can be used and our limited knowledge and also budget constraints made the research laborious. But with perseverance and determination, we managed to develop find the right one and implement it in a running workflow. The inclusion of the sentiment analysis addes immense value to helpica.ch, enhancing its capabilities and user experience. The project demonstrated the immense promise of AI, especially with the successful integration of sentiment analysis. We witnessed firsthand how this technology can provide valuable insights for helpica.ch and significantly improve its performance.

None of this would have been possible without the great collaboration among all the lecturers and coaches involved in the project. Their support, guidance, and expertise were instrumental in overcoming challenges and achieving our goals. 
A special mention goes to Maja, whose tireless support significantly contributed to our success.

We enjoyed continuing to work on the helpica.ch project, as this start-up was the outcome of the Agile Business Analysis module in the previous semester. Building upon our prior experience, we are proud of the progress made and the positive impact we have created.
We look forward to sharing our results with the rest of the helpica.ch team and refining and expanding its capabilities in the future.

