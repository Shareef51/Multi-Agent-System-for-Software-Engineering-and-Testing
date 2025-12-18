

# 🧠 Multi-Agent-System-for-Software-Engineering-and-Testing

## 📌 Overview

This repository implements an **AI-driven Python development and testing workflow** where two virtual agents — **Developer** and **Tester** — collaborate iteratively to produce **high-quality, well-tested Python code**.

The system is designed to:

* Generate optimal Python solutions for a given problem
* Create **exhaustive unit test cases**
* Evaluate code quality and correctness
* Reflect on failures and improve code iteratively
* Score each iteration objectively
* Produce detailed testing reports and critiques

This framework is ideal for:

* AI Engineer interview projects
* Auto-grading systems
* Code quality benchmarking
* Agentic AI demonstrations
* Teaching TDD (Test-Driven Development)

---

## 🏗️ System Architecture

### 🔹 Developer Agent

Responsible for:

* Writing the **initial Python solution**
* Refining code based on tester feedback
* Handling **all edge cases**
* Improving performance, readability, and maintainability
* Adding **clear docstrings and inline comments**

### 🔹 Tester Agent

Responsible for:

* Designing **exhaustive unit test cases**
* Running tests against the developer’s code
* Identifying edge cases, failures, and regressions
* Producing a **detailed unit test report**
* Scoring the solution objectively
* Recommending improvements
* Triggering reflections if failures exist

---

## 🔁 Iterative Reflection Loop

The system follows a controlled reflection cycle:

* **max_reflections** → Maximum number of allowed improvement cycles
* **reflection_count** → Current iteration index

### Iteration Flow:

1. Developer submits Python code
2. Tester executes unit tests
3. Tester generates:

   * Pass/fail summary
   * Coverage analysis
   * Edge case failures
4. Tester assigns:

   * **Code Quality Score (0–10)**
   * **Unit Test Pass Percentage**
5. Developer refines code
6. Loop continues until:

   * All tests pass, or
   * `max_reflections` is reached

---

## 🧪 Unit Testing Strategy

The tester follows **industry-grade testing standards**:

### ✅ Test Coverage Includes:

* Normal input cases
* Boundary conditions
* Invalid inputs
* Type mismatches
* Null / empty values
* Large input stress tests
* Performance constraints
* Exception handling
* Regression scenarios

### 📊 Test Report Contains:

* Total test cases executed
* Passed / failed count
* Failure reasons
* Stack traces (if applicable)
* Edge cases uncovered
* Recommendations for fixes

---

## 📈 Scoring System

Each iteration is scored using two metrics:

### 🔹 1. Code Quality Score (0–10)

Based on:

* Correctness
* Readability
* Pythonic style
* Modularity
* Docstrings & comments
* Error handling
* Performance
* Edge case handling

### 🔹 2. Unit Test Pass Percentage

```
(pass_count / total_test_cases) × 100
```

### 🧮 Final Evaluation Snapshot:

| Metric               | Value         |
| -------------------- | ------------- |
| Code Quality Score   | 0–10          |
| Test Pass Percentage | 0–100%        |
| Reflection Count     | Current / Max |

---

## 📝 Critique & Recommendations

If **any test cases fail**, the tester generates:

* A **critique section** highlighting weaknesses
* Root-cause analysis
* Specific refactoring suggestions
* Missing edge cases
* Design improvements





<img width="1678" height="761" alt="image" src="https://github.com/user-attachments/assets/5c2a8357-f6b7-419a-a2b4-eb041996081a" />
