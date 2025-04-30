# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:                                                                            
### REGISTER NUMBER : 212222230152
### Aim:
To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

### Algorithm:  1. Direct Instruction Prompts
Objective: Guide the chatbot to respond concisely to customer inquiries.
Prompt Pattern:
Prompt: "When a customer asks for the status of their order, reply with: 'Your order is currently being processed and will be delivered by [date].'"
2. Contextual Prompting
Objective: Incorporate specific context to provide detailed answers based on the user’s previous interaction.
Prompt Pattern:
Prompt: "If the customer previously mentioned that they haven’t received their order, say, 'I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly.'"
3. Persona-Based Prompting
Objective: Design the chatbot to adopt a specific persona, making the interaction more engaging.
Prompt Pattern:
Prompt: "Pretend you are a friendly, helpful customer service representative. Use a conversational tone, such as 'Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!'"
4. Few-Shot Prompting
Objective: Teach the AI how to respond using a few examples, enabling it to generalize for similar situations.
Prompt Pattern:
Prompt: "Here are some examples of how to handle technical questions:
'My phone isn't charging.' → 'Have you tried using a different cable? If that doesn’t work, it may be an issue with the port.'
'The screen is flickering.' → 'It sounds like a display issue. Have you tried restarting the device?'
Now, respond to: 'My app keeps crashing.'"
5. Chain of Thought Prompting
Objective: Use a step-by-step reasoning approach for resolving more complex or technical issues.
Prompt Pattern:
Prompt: "When a customer reports their laptop overheating, guide them through the following steps:
Ask if they are using the laptop on a soft surface.
Suggest moving the laptop to a flat, hard surface for better airflow.
Ask if they’ve cleaned the vents recently.
Recommend restarting the device to see if the issue persists.
Now, solve: 'My laptop fan is making a loud noise.'"
6. Instruction with Constraints
Objective: Instruct the chatbot to provide assistance while adhering to specific constraints (e.g., response length or tone).
Prompt Pattern:
Prompt: "Respond to order inquiries in no more than 50 words and avoid using technical jargon. For example, 'Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else.'"
7. Reflective Prompting
Objective: Ensure that the chatbot reflects the user’s query back to them before providing a response, reducing misunderstandings.
Prompt Pattern:
Prompt: "When a customer asks for help, first reflect their question back to them. For example, if they ask 'How can I reset my password?' respond with 'You're asking how to reset your password, correct? Here’s how you can do it.'"
Result: The various types of Prompts are executed successfully.
## Use Case: Customer Support Chatbot
### Scenario:
A customer service chatbot designed to assist users with product troubleshooting, order tracking, and answering general inquiries. The chatbot must handle the following common scenarios effectively:

Product Troubleshooting: Help customers resolve issues related to malfunctioning products.

Order Tracking: Provide updates on the status of customer orders.

General Inquiries: Answer general questions related to the company's products or services.

The chatbot will use different prompting techniques to guide its responses in each case.

### 1. Straightforward Prompting Technique
Prompt: Product Troubleshooting
Prompt to ChatGPT and Bard:
"My phone isn’t turning on. What should I do?"

### Response from ChatGPT:
"First, try holding the power button for 10 seconds to force a restart. If that doesn't work, check if the battery is charged. If it's still not turning on, try plugging the phone into a charger for a few minutes to see if the battery is completely drained."

### Response from Bard:
"Try pressing and holding the power button for 10 seconds. If that doesn’t work, plug your phone into a charger for 10-15 minutes and then try turning it on again. If the issue persists, your device may need a professional diagnosis."

Prompt: Order Tracking
Prompt to ChatGPT and Bard:
"What’s the status of my order? The order number is 12345."

### Response from ChatGPT:
"Your order #12345 is currently being processed and is expected to be shipped by [date]. You will receive a notification once it has been dispatched. Thank you for your patience!"

### Response from Bard:
"Order #12345 is on its way! It is expected to be shipped out by [date]. We will notify you once it’s on the move."

Prompt: General Inquiry
Prompt to ChatGPT and Bard:
"Can you tell me more about the warranty on your laptops?"

### Response from ChatGPT:
"Our laptops come with a standard 1-year warranty, covering hardware defects and manufacturing issues. For further details, please refer to the warranty policy available on our website or contact our support team for assistance."

### Response from Bard:
"All laptops are covered by a 1-year warranty for any manufacturing defects or hardware malfunctions. You can find more details about our warranty coverage and the claims process on our website or contact our customer service for further help."


## 2. Preceding Question Prompting Technique
Prompt: Product Troubleshooting (Preceding Question)
Prompt to ChatGPT and Bard:
"My laptop is making strange noises. What should I do?"
### ChatGPT:
"I’ll help you with that. First, can you tell me if the noise happens when the laptop is idle or during specific tasks? Also, does the sound come from the fan, speakers, or elsewhere?"

### Bard:
"I can assist with that. Does the noise occur when you're using certain programs or when the laptop is idle? Is it a grinding or clicking sound, or more of a whirring noise from the fan?"

## Prompt: Order Tracking (Preceding Question)
Prompt to ChatGPT and Bard:
"Where is my order?"
### ChatGPT:
"I’d be happy to check that. Can you provide me with your order number to get started?"

### Bard:
"Sure! Can you please share your order number so I can look up the current status?"
1. Straightforward Prompting Technique
Product Troubleshooting:
Prompt: "My phone isn’t turning on. What should I do?"

### ChatGPT:

Accuracy: 5/5 — The troubleshooting steps are accurate and common for phone issues.

Clarity: 5/5 — The response is clear and easy to follow.

Relevance: 5/5 — It directly addresses the customer's issue.

User-Friendliness: 5/5 — The tone is helpful and comforting.

### Bard:

Accuracy: 5/5 — The solution is correct, focusing on common troubleshooting methods.

Clarity: 5/5 — Very clear and actionable steps.

Relevance: 5/5 — The response directly addresses the issue raised by the customer.

User-Friendliness: 4/5 — A bit more formal but still approachable.

Evaluation: Both ChatGPT and Bard provided excellent responses. They each presented clear, actionable solutions. Bard’s response was slightly more formal, while ChatGPT’s was friendlier, but both were effective.

Final Score (each): 19/20

### Order Tracking:
Prompt: "What’s the status of my order? The order number is 12345."

### ChatGPT:

Accuracy: 5/5 — It correctly explains the status and expected shipping date.

Clarity: 5/5 — The message is concise and well-structured.

Relevance: 5/5 — Directly answers the query.

User-Friendliness: 5/5 — Clear and courteous tone.

### Bard:

Accuracy: 5/5 — It provides accurate and standard response about order tracking.

Clarity: 5/5 — It is straightforward.

Relevance: 5/5 — It directly addresses the question.

User-Friendliness: 4/5 — Professional, but slightly less engaging compared to ChatGPT.

Evaluation: Both responses were equally effective in providing order status. ChatGPT’s tone was slightly more engaging, while Bard's was more formal but still effective.

Final Score (each): 19/20

General Inquiry:
Prompt: "Can you tell me more about the warranty on your laptops?"

### ChatGPT:

Accuracy: 5/5 — Provides a correct and comprehensive response.

Clarity: 5/5 — The message is very clear.

Relevance: 5/5 — Answers the customer’s question directly.

User-Friendliness: 5/5 — The tone is approachable and helpful.

### Bard:

Accuracy: 5/5 — Gives a clear and correct description of the warranty.

Clarity: 5/5 — Clear and easy to understand.

Relevance: 5/5 — It directly addresses the query.

User-Friendliness: 4/5 — Slightly formal tone but still polite and informative.

Evaluation: Both responses were on point with clear and accurate information. ChatGPT’s response was a bit more casual and engaging, whereas Bard's response was slightly more formal.

Final Score (each): 19/20



## 2. Preceding Question Prompting Technique
Product Troubleshooting (Preceding Question):
Prompt: "My laptop is making strange noises. What should I do?"

### ChatGPT:

Accuracy: 5/5 — The question helps guide the troubleshooting steps.

Clarity: 5/5 — The follow-up questions are well-phrased and lead to clear steps.

Relevance: 5/5 — Focuses on gathering more details to provide accurate assistance.

User-Friendliness: 5/5 — The response is empathetic and conversational.

### Bard:

Accuracy: 5/5 — Provides helpful follow-up questions to guide the troubleshooting.

Clarity: 5/5 — The questions are clear and easy to understand.

Relevance: 5/5 — Directly addresses the issue by gathering more context.

User-Friendliness: 4/5 — The tone is professional but slightly more formal than ChatGPT’s.

Evaluation: Both responses use follow-up questions effectively to gather more context for troubleshooting. ChatGPT's response is slightly more empathetic and conversational, while Bard’s is more formal.

Final Score (ChatGPT): 19/20
Final Score (Bard): 18/20

### Overall Evaluation Summary:
Final Assessment:
Winner: ChatGPT

### Reason: 
ChatGPT consistently provided responses that were not only accurate and clear but also user-friendly with a more empathetic and conversational tone. It excelled in making the interaction feel personal and approachable.

### Bard:
Bard performed very well, especially in terms of accuracy and clarity. However, its tone was more formal, which may not always be as engaging as ChatGPT's more casual and friendly approach


# Result: 
Thus the Prompts were exected succcessfully .

