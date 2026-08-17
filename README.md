# oceantrash-nz.github.io
A website I have created for my ANI Exhibition Project

Gemini Prompt:
Create a single-file HTML survey with a deep navy ocean theme.

Design & Layout:

The background should be a gradient from a normal navy blue to a darker navy blue.

Add visual decorations on the sides featuring vertical waves and animated floating bubbles.

At the top of the page, include a big white text title and a subtitle.

The main content should be in a centralized box.

Flow & Animation:

The page should start by showing a confirmation box that says: 'This data will be sent to Students at Auckland Normal Intermediate, and the data being sent will be anonymous.'

Below this text, add a button that says 'Yes, I understand'.

When the user clicks this button, play a smooth tween animation where the confirmation box slides out to the left, and the actual survey box slides in from the right to replace it.

Survey Questions:

The first question is 'Do you litter?' with 'Yes' and 'No' radio buttons.

The follow-up questions and the submit button must remain hidden until the user selects 'Yes' or 'No'.

If they select 'Yes', show a question saying 'Why do you do it?' with a text area below it.

If they select 'No', show a question saying 'Why do you think people do it?' with a text area below it.

Below that, show a final question saying 'How could we prevent it from happening?' with another text area.

At the bottom, add a button that just says 'Submit'.

Functionality & Anti-Abuse:

When the user clicks Submit, send all the gathered information to a Discord webhook using a JSON payload. Keep the webhook URL as a constant variable in the JavaScript so I can easily configure it in the code.

Anti-abuse feature: Use the browser's localStorage to prevent duplicate submissions. When a user successfully submits the survey, save a completion flag in local storage.

When the page first loads, check if this flag exists in local storage. If it does, hide the confirmation/survey boxes entirely and instead display a message saying 'You have already completed this survey. Thank you!' so they cannot answer it again."
