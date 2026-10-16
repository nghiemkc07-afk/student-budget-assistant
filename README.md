# Student Budget Assistant

## Project Overview

Student Budget Assistant is a Python-based application designed to help university students manage their monthly budgets.

The application calculates total expenses, remaining balance, and budget status. It also uses Google's Gemini AI to analyse spending patterns and answer budgeting questions based on financial information entered by the user.

## Main Features

- Calculate total monthly expenses and remaining balance.
- Identify whether a student is within or over budget.
- Analyse expenses across five categories: Food, Transport, Rent, Shopping, and Other.
- Provide AI-generated budgeting advice through Gemini.
- Allow users to ask their own financial questions.
- Reject negative financial inputs.
- Handle temporary Gemini API errors.
- Provide a simple interactive interface using Gradio.

## Technologies Used

- Python
- Google Colab
- Google Gemini API
- Gradio
- GitHub

## Sample Input and Output

**Example Input**

| Category | Amount (AUD) |
|---|---:|
| Monthly Income | 2,000 |
| Food | 400 |
| Transport | 300 |
| Rent | 700 |
| Shopping | 200 |
| Other | 100 |

**Example Output**

- Total Expenses: AUD 1,700
- Remaining Balance: AUD 300
- Budget Status: Within Budget

**Example User Question**

How can I save $200 more per month?

**Example Gemini Response (summarised)**

The assistant suggests reducing Shopping by AUD 100, Food by AUD 60, and Transport by AUD 40. These adjustments could increase the remaining monthly balance from AUD 300 to AUD 500.

## How to Run the Application

1. Open `finance_assistant.ipynb` in Google Colab.
2. Create a Gemini API key using Google AI Studio.
3. Open the Secrets panel in Colab.
4. Add the key under the name `GEMINI_API_KEY` and enable notebook access.
5. Run the notebook cells in order.
6. Open the Gradio interface using the generated link.
7. Enter monthly income, expenses, and a budgeting question.
8. Click Submit to receive the budget calculation and Gemini's response.

## Testing and Error Handling

The application has been tested with normal budgets, overspending scenarios, negative expense inputs, and AI-generated responses to budgeting questions.

The application also includes error handling for temporary Gemini API failures, allowing budget calculations to remain available when AI responses cannot be generated.

## Limitations

- Gemini responses depend on API availability.
- The assistant relies on user-entered financial data.
- The application does not connect to bank accounts.
- The assistant provides general budgeting guidance rather than professional financial advice.
