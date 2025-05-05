# dotcursor

This repository stores the shared `.cursor` folders used by our technical team in
the [Cursor IDE](https://www.cursor.sh/).
These rules help define and automate coding patterns and actions of AI agents.

## 📁 Folder Structure
Each subdirectory typically represents a separate `.cursor` folder used for a specific project,
tech stack, or shared configuration pattern.


## 🧠 Purpose
- Maintain a **centralized, version-controlled** source of `.cursor` folders.
- Promote **consistency across teams and repositories**.
- Enable **quick onboarding** by simply linking or copying rules into Cursor.

## 🚀 Usage
1. Clone or pull this repository.
2. Copy or symlink the relevant `.cursor` folder into your local project root.
3. Cursor will automatically detect and apply the rules.

## 🛠️ .rules projects we have here

### Tests automation 

This set of rules automatically produces test cases according to given specifications and test case IDs.
Before running the rules, you have to 

1. Clone our Octa main repository.
2. Clone the repository with the test cases.
3. Gain the access to the Testrails where the test cases are stored.

When you are prompting  the Cursor agent, the best way is to copy the entire test case with ID
to chat and askt the agent to produce the test case according to the given specification.

For example:

```
Please write for me a code for test case C776 'Verify that password must be at least 8 characters long'.

Steps to reproduce:
- Navigate to the login page: https://staging.weareocta.com/login.
- Enter a password with fewer than 8 characters.
- Click ""Login.""

The system should show an error message: ""Password must be at least 8 characters long.""

```

