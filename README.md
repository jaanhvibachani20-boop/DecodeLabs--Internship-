# Prompt Engineering Project 1: Zero-Shot & Few-Shot Data Extraction

## Objective

Design a deterministic prompt that extracts structured information from unstructured customer support emails and returns the output in a strict JSON format.

## Extracted Fields

```json
{
  "customer_name": "string",
  "order_number": "string",
  "complaint_type": "string",
  "severity_level": 0,
  "contact_phone": "string | null"
}
```

## Techniques Used

- Delimiter-Based Prompting (`###`)
- Few-Shot Learning
- JSON Schema Enforcement
- Null Fallback Handling
- Deterministic Prompt Design

## Repository Structure

```text
├── prompts/
├── test_cases/
├── outputs/
├── docs/
└── README.md
```

## Test Cases

1. Standard Complaint Extraction
2. Missing Phone Number (`null` handling)
3. Prompt Injection Attempt

## Sample Output

```json
{
  "customer_name": "Priya Sharma",
  "order_number": "ORD78901",
  "complaint_type": "Damaged Product",
  "severity_level": 3,
  "contact_phone": null
}
```

## Key Learnings

- Few-Shot Prompting
- Delimiter Usage
- Structured Data Extraction
- Hallucination Prevention
- Consistent JSON Generation
