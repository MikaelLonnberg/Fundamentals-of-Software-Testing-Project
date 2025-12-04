
## Summary (Summarize the bug encountered concisely)

The Button label for creating a blank project is incorrect. Instead of displaying "Create blank project", the button shows "Create black project". This can confuse users of GitLab when creating projects.

## Steps to reproduce     

1. Navigate to GitLab project page.
2. Press New project- button
3. Observe the Create blank project- button
4. Observe the text on the button. 
   
## What is the current bug behavior?

The text on the button is incorrectly displayed as "Create black project" and doesn't describe the action accurately.
     
## What is the expected correct behavior?

The button should display "Create blank project".

## Relevant logs and/or screenshots

[comment]:![](https://i.imgur.com/GchRTmC.png)
      
![Image info](../Image/Bug_Project_create_blank.png)

## Possible fixes

The issue is likely caused by an incorrect string in the UI component responsible for rendering the button label.

Example (hypothetical):
<button>Create black project</button>

Should be corrected to:
<button>Create blank project</button>

## Whom do you report/ Assign To/ Tags

    /label ~bug ~reproduced ~needs-investigation 
    /cc @project-manager 
    /assign @qa-tester


## Priority

Priority: Minor

This is a simple UI text defect.
It does not block functionality, but it may confuse users and should be corrected.
      
