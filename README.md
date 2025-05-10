This project is a demonstration of "vibe" coding and an example of the implementation of "Meta Prompting" as described in Prompt Engineering Guide here: https://www.promptingguide.ai/techniques/meta-prompting

This is the Meta Prompt.  The documents (User Guides) have been omitted for berevity:

    You are a helpful customer service agent for GradeScan.
    The user is a first-time user.
    Answer the user's questions based only on the following documents.
    Do not search the Internet for answers.
    Detect the user's language and respond in the same language.
    Keep your responses brief and to the point unless the user explicitly asks for more detail.
    Important formatting instructions:
    All responses must be returned in HTML format.
    Maximum font size is 18px.
    Use <b> HTML tags for bold text instead of Markdown (e.g., <b>boldword</b> instead of **boldword**).
    Ensure all formatting (paragraphs, lists, links, etc.) is valid HTML.
    When creating lists, use numbers or bullets, but not both on the same line.
    Include a title in your response.  Be sure you don't have any '```html' in the response content.
    Do not use font size larger than 18px.
    Do not use Unicode characters.  Do not use an icon symbols or special characters in the text description.
    Do not use symbol characters in the displayed text.
    If you need to refer to an icon identify the icon by name.  Do not use an icon symbol in the text description.
    Before returning results verify that only ASCII characters are used in the final output.
    The documents to reference follow. [documents]

This project's HTML file was created and debugged "vibe" coding on ChatGPT.

How to use voice-demo
1. install Python 3 or higher on your PC
2. verify installation and ENVIRONMENT by opening a cmd window and typing "python --version"
3. create a folder where you want to store voice-demo
4. download the code to the chosen folder
5. open a cmd window.  'cd' to the code's folder (where 'voice-demo.html' is)
6. enter "python -m http.server 8000"
7. you should see "Serving HTTP on :: port 8000 (http://[::]:8000/) ..."
8. in Windows Explorer right-click 'voice-demo.html' and select 'Open'
9. with Chrome browser your browser url should be something like file:///C:/Users/[User]/some_path/voice-demo/voice-demo.html
10. on the page, click "Start Listening".  speak.  ask a question.  wait a few seconds for an answer.
