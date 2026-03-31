# QA Test Case Generator Agent 

## Problem

Test case creation is manual, time-consuming, and often misses edge cases. This leads to incomplete coverage and inconsistent quality across test suites.

---

## Solution

An AI-powered agent that generates structured, comprehensive test cases from:

* User stories
* API specifications
* Functional requirements

---

## Capabilities

* Generates:

  * Positive scenarios
  * Negative scenarios
  * Edge cases
* Adds test metadata:

  * Priority (High/Medium/Low)
  * Tags (Smoke, Regression, Sanity)
* Ensures coverage across:

  * Input validation
  * Error handling
  * Boundary conditions

---

## How it Works

Input → LLM → Scenario Expansion → Structured Test Cases

---

## ▶Usage

```bash
pip install -r requirements.txt
python src/agent.py
```

---

## Example

### Input

```json
{
  "user_story": "User logs in using email and password"
}
```

### Output

```json
{
  "test_cases": [
    {
      "title": "Valid login",
      "priority": "High",
      "tag": "Smoke"
    },
    {
      "title": "Invalid password",
      "priority": "High",
      "tag": "Regression"
    },
    {
      "title": "Empty email field",
      "priority": "Medium",
      "tag": "Negative"
    }
  ]
}
```

---

## Value

* Reduces manual effort in test design
* Improves coverage and consistency
* Accelerates test planning cycles

---

## QA Agents Hub

👉 https://github.com/YOUR_USERNAME/qa-agents
