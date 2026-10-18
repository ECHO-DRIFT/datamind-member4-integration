# DataMind Manufacturing - System Architecture

## 1. Project Overview

DataMind Manufacturing is an AI-powered conversational
data analysis system for manufacturing operations.

It allows factory managers to ask questions in natural
language and receive evidence-backed answers from actual
manufacturing data.

## 2. System Flow

User
  ↓
Streamlit Application
  ↓
Google Gemma
  ↓
SQL Query
  ↓
Snowflake Database
  ↓
Query Result
  ↓
Evidence + Explanation
  ↓
User

## 3. Team Modules

### Member 1 - Database & Snowflake

Responsible for:

- Snowflake database
- Manufacturing tables
- Sample data
- SQL queries
- Database validation

### Member 2 - AI & Gemma

Responsible for:

- Gemma setup
- Natural-language understanding
- SQL generation
- Ambiguous question handling
- Unsupported request handling

### Member 3 - Application & Dashboard

Responsible for:

- Streamlit application
- Chat interface
- Manufacturing dashboards
- SQL and evidence display

### Member 4 - Integration, Testing & Demo

Responsible for:

- Integrating all modules
- Functional testing
- Ground-truth verification
- Edge-case testing
- Documentation
- Demo preparation

## 4. End-to-End Process

1. User enters a manufacturing question.
2. Streamlit sends the question to the AI module.
3. Gemma interprets the question.
4. Gemma generates a SQL query or requests clarification.
5. SQL is sent to Snowflake.
6. Snowflake executes the query.
7. The result is returned to the application.
8. The application displays the result and supporting evidence.
9. The AI provides an explanation based only on the available data.

## 5. Testing Focus

The integrated system will be tested for:

- Correct answers
- Incorrect or invalid SQL
- Missing data
- Ambiguous questions
- Unsupported questions
- End-to-end communication
- Evidence-backed responses
