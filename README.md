# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:                                                                            
### REGISTER NUMBER : 212222230152
### Aim:
To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

## Algorithm: 

## 1. Direct Instruction Prompts
### Objective: Guide the chatbot to respond concisely to customer inquiries.

### Prompt Pattern:

### Prompt:
"When a customer asks for the status of their order, reply with: 'Your order is currently being processed and will be delivered by [date].'"

## 2. Contextual Prompting

Objective: Incorporate specific context to provide detailed answers based on the user’s previous interaction.

### Prompt Pattern:

### Prompt: 
"If the customer previously mentioned that they haven’t received their order, say, 'I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly.'"

## 3. Persona-Based Prompting

### Objective: Design the chatbot to adopt a specific persona, making the interaction more engaging.

### Prompt Pattern:

### Prompt: 
"Pretend you are a friendly, helpful customer service representative. Use a conversational tone, such as 'Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!'"

## 4. Few-Shot Prompting

### Objective: Teach the AI how to respond using a few examples, enabling it to generalize for similar situations.

### Prompt Pattern:

### Prompt: 
"Here are some examples of how to handle technical questions:

'My phone isn't charging.' → 'Have you tried using a different cable? If that doesn’t work, it may be an issue with the port.'
'The screen is flickering.' → 'It sounds like a display issue. Have you tried restarting the device?'

Now, respond to: 'My app keeps crashing.'"

## 5. Chain of Thought Prompting

### Objective: Use a step-by-step reasoning approach for resolving more complex or technical issues.

### Prompt Pattern:

### Prompt: "When a customer reports their laptop overheating, guide them through the following steps:

Ask if they are using the laptop on a soft surface.

Suggest moving the laptop to a flat, hard surface for better airflow.

Ask if they’ve cleaned the vents recently.

Recommend restarting the device to see if the issue persists.

Now, solve: 'My laptop fan is making a loud noise.'"

## 6. Instruction with Constraints

### Objective: Instruct the chatbot to provide assistance while adhering to specific constraints (e.g., response length or tone).

### Prompt Pattern:

### Prompt:
"Respond to order inquiries in no more than 50 words and avoid using technical jargon. For example, 'Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else.'"

## 7. Reflective Prompting

### Objective: Ensure that the chatbot reflects the user’s query back to them before providing a response, reducing misunderstandings.

### Prompt Pattern:

### Prompt:
"When a customer asks for help, first reflect their question back to them. For example, if they ask 'How can I reset my password?' respond with 'You're asking how to reset your password, correct? Here’s how you can do it.'"

Result: The various types of Prompts are executed successfully.
### 1. Direct Instruction Prompt
#### Prompt:
"When a customer asks about delivery status, respond with:
'Your delivery is on its way and should arrive by [date]. Let us know if you need anything else.'"
| Tool       | Output                                                                                                   |
| ---------- | -------------------------------------------------------------------------------------------------------- |
| **Gemini** | "Your delivery is on its way and should arrive by May 17th. Let us know if you need anything else."      |
| **Cohere** | "Your order is en route and will be delivered by May 17. If you have questions, feel free to reach out." |
✅ Both tools provide accurate, direct answers with slightly varied wording. Cohere adds a slightly more formal tone.

### 2. Contextual Prompting
#### Prompt:

"If the customer already mentioned their item was delayed, respond with:
'I understand you’ve experienced a delay. Let me review your order and provide an updated ETA.'"
| Tool       | Output                                                                                                   |
| ---------- | -------------------------------------------------------------------------------------------------------- |
| **Gemini** | "I understand you’ve experienced a delay. Let me review your order and provide an updated ETA."          |
| **Cohere** | "Thanks for your patience. I see you've faced a delay—I'll check your order now and update you shortly." |
✅ Gemini sticks to instructions exactly. Cohere offers a slightly more conversational variation while maintaining context.

### 3. Persona-Based Prompting
#### Prompt:

"Act like a cheerful and friendly support assistant. Say something like:
'Hi there! 😊 I’m here to help with anything you need. Let’s solve this together!'"
| Tool       | Output                                                                                                              |
| ---------- | ------------------------------------------------------------------------------------------------------------------- |
| **Gemini** | "Hi there! 😊 I’m here to help with anything you need. Let’s solve this together—what can I assist you with today?" |
| **Cohere** | "Hey! 😄 So glad you reached out. Let’s figure this out together—what can I do for you today?"                      |
✅ Gemini stays close to the original tone. Cohere adds more personality and informal warmth, making it feel more human.

### 4. Few-Shot Prompting
#### Prompt:
Examples:

"My laptop isn't turning on." → "Try holding the power button for 10 seconds. If that doesn’t work, check your charger."

"The printer is offline." → "Restart your printer and reconnect it to Wi-Fi."

Now respond to:
"My mouse isn’t responding."
| Tool       | Output                                                                                                                  |
| ---------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Gemini** | "Try reconnecting the mouse or replacing the battery if it's wireless. Also, check the USB port or Bluetooth settings." |
| **Cohere** | "Make sure the mouse is turned on. If it’s wireless, try new batteries. If wired, try another USB port."                |
✅ Both tools successfully apply example logic. Gemini is slightly more technical, while Cohere offers clearer steps for general users.

### 📊 Performance Comparison Table
| Prompt Type            | Gemini Highlights               | Cohere Highlights                     | Best Use Case                   |
| ---------------------- | ------------------------------- | ------------------------------------- | ------------------------------- |
| **Direct Instruction** | Followed template precisely     | Slightly more professional tone       | Gemini for strict adherence     |
| **Contextual Prompt**  | Mirrors prior context well      | Adds warmth and personalization       | Cohere for empathetic responses |
| **Persona-Based**      | Friendly and clear              | More enthusiastic and casual          | Cohere for engaging tone        |
| **Few-Shot**           | Logical, well-reasoned solution | Simplified explanation, user-friendly | Tie – Both handled it well      |

### 🔄 Prompt, Input, and AI Response Table:

| **#** | **Prompt Type**          | **Prompt**                                                                                                                                                                                                          | **Customer Input**                                                                | **Gemini Response**                                                                                                                       | **Cohere Response**                                                                                                                  |
| ----- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| 1     | **Direct Instruction**   | "When a customer asks about delivery status, respond with: 'Your delivery is on its way and should arrive by \[date]. Let us know if you need anything else.'"                                                      | “Can you tell me when my order will arrive?”                                      | "Your delivery is on its way and should arrive by May 17th. Let us know if you need anything else."                                       | "Your order is en route and will be delivered by May 17. If you have questions, feel free to reach out."                             |
| 2     | **Contextual Prompting** | "If the customer already mentioned their item was delayed, respond with: 'I understand you’ve experienced a delay. Let me review your order and provide an updated ETA.'"                                           | “It’s been 4 days and my package still hasn’t come. I’m starting to get worried.” | "I understand you’ve experienced a delay. Let me review your order and provide an updated ETA."                                           | "Thanks for your patience. I see you've faced a delay—I'll check your order now and update you shortly."                             |
| 3     | **Persona-Based Prompt** | "Act like a cheerful and friendly support assistant. Say something like: 'Hi there! 😊 I’m here to help with anything you need. Let’s solve this together!'"                                                        | “Hey, I’m new here. Can you help me track my first order?”                        | "Hi there! 😊 I’m here to help with anything you need. Let’s solve this together—can you share your order number?"                        | "Hey! 😄 I'm super glad you're here! Let’s check on your order—just share your order number with me!"                                |
| 4     | **Few-Shot Prompting**   | **Examples:**<br>• “My laptop isn't turning on.” → “Try holding the power button for 10 seconds...” <br>• “The printer is offline.” → “Restart your printer...”<br>**Now respond to:** “My mouse isn’t responding.” | “Hi, my wireless mouse stopped working suddenly. What should I do?”               | "Try replacing the mouse battery and reconnecting it via Bluetooth. If that doesn’t work, check if the USB receiver is working properly." | "Check if the mouse is powered on. Try replacing the battery or reconnecting the Bluetooth. If needed, re-pair it with your device." |

### 🧠 Insights:
Different prompt types are best suited to specific use cases.

Using multiple AI tools helps optimize performance across emotional tone, accuracy, and engagement potential.

Persona-based and contextual prompting benefit most from tools like Cohere that prioritize emotional connection.

Gemini is preferred when instruction clarity and structure are the priority.



# Result: 
Thus the Prompts were exected succcessfully .

