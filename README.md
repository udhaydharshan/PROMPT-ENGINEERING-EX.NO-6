# Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

# Date:14-5-2026
# Register number:212225230286
# Aim: Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools

#AI Tools Required:

# Explanation:
Experiment the persona pattern as a programmer for any specific applications related with your interesting area. 
Generate the outoput using more than one AI tool and based on the code generation analyse and discussing that. 

# Conclusion:
```
The Persona Prompt Pattern is a prompting technique where the AI is instructed to assume a specific role or identity (persona) while responding. By assigning a persona such as “expert programmer”, “software architect”, or “IoT developer”, the AI’s output becomes more domain-specific, structured, and practical.

In this experiment, the persona pattern is applied in the field of Software Development, specifically focusing on a Web-based Student Management System, which is an area of interest due to its relevance in real-world academic and enterprise applications.
```
Objective of the Experiment 
```
The objectives are:

To experiment with the Persona Prompt Pattern

To generate programming code using multiple AI tools

To compare and analyze the generated code

To discuss how different AI tools perform under the same programmer persona
```
3. Selected Application Area)
```
Application Chosen:
 Web-based Student Management System

Reason for Selection:

Common real-world application

Involves backend logic, databases, and APIs

Suitable for comparing code quality and structure
```
4. Persona Definition (3 Marks)
```
The persona used in this experiment:

“You are an experienced full-stack programmer with expertise in Python, Flask, and REST APIs. Write clean, secure, and scalable code.”

This persona ensures:

Industry-level coding practices

Proper comments and structure

Focus on scalability and security
```
5. AI Tools Used (4 Marks)
```
Two AI tools were used for experimentation:

AI Tool 1: ChatGPT

Strengths: Clean explanations, structured code, comments

Focus on readability and best practices

AI Tool 2: Google Gemini / Copilot-style AI

Strengths: Concise code, practical implementation

Focus on quick development and minimal explanations
```
6. Prompt Used (Persona-Based Prompt) 
```
Prompt:

“You are an experienced full-stack programmer. Develop a REST API using Python Flask for a Student Management System that allows adding and viewing students. Use best coding practices and include comments.”
```
7. Output from AI Tool 1 – ChatGPT (Code Generation) 
from flask import Flask, request, jsonify
```
app = Flask(_name_)

# In-memory student database
students = []

@app.route('/add_student', methods=['POST'])
def add_student():
    data = request.json
    student = {
        "id": len(students) + 1,
        "name": data["name"],
        "course": data["course"]
    }
    students.append(student)
    return jsonify({"message": "Student added successfully"}), 201

@app.route('/students', methods=['GET'])
def get_students():
    return jsonify(students), 200

if _name_ == '_main_':
    app.run(debug=True)


Observations:

Clear structure and comments

Beginner-friendly

Easy to understand and modify

Suitable for academic purposes
```
8. Output from AI Tool 2 – Gemini / Copilot-style AI (Code Generation)
from flask import Flask, request, jsonify
```
app = Flask(_name_)
students = []

@app.post("/students")
def create_student():
    students.append(request.json)
    return {"status": "created"}, 201

@app.get("/students")
def list_students():
    return jsonify(students)

app.run()

```

Observations:
```
More concise

Less commenting

Faster to implement

Suitable for experienced developers

9. Comparative Analysis 
Aspect	ChatGPT Output	Gemini / Copilot Output
Code Readability	High	Medium
Comments	Detailed	Minimal
Scalability	Moderate	Moderate
Beginner Friendly	Yes	No
Development Speed	Medium	High
```
10. Discussion
```
The Persona Prompt Pattern significantly improved the quality of responses from both AI tools. By defining the AI as an experienced programmer, the generated code followed:

Logical structure

REST API standards

Clean function separation

Using multiple AI tools highlighted their differences:

ChatGPT focuses on learning, clarity, and explanation

Gemini/Copilot focuses on speed and efficiency

This shows that persona-based prompting works across platforms but outputs vary based on tool design.
```
 
```
The experiment successfully demonstrates that the Persona Prompt Pattern is highly effective in programming-related tasks. When applied to a Student Management System, it resulted in:

Better code quality

Context-aware responses

Improved relevance

Using more than one AI tool provides flexibility:

One tool for learning and documentation

Another for rapid development

Thus, persona-based prompting is a powerful technique for real-world software development and academic experimentation.


```
# Result: The corresponding Prompt is executed successfully.
