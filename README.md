# Excel-Loan-Payment-Projection
# The Challenge

---

Given three proposals from three different banks for a loan, calculate:

- Monthly Payment
- Total Cost of loan
- Total Interest amount

Present the best offer according to the data.

# How I approached it

---

## Monthly Payment

I needed help understanding financial terms. So I used CHATGPT to help me.

💡 I have an Excel file with the Loan amount, annual interest rate, and Loan Period in years. What formula can I use in Excel to calculate the monthly payment?

💡 **PMT(rate, nper, pv, [fv], [type])**

- Where “rate” is the interest rate (Since the file had an annual interest rate, I have to divide that value by 12
- Where “nper” is the number of payments (Since the file had a yearly nper, I have to multiply by 12 to get the number of months;
- “Pv” which stands for the actual amount of the Loan

💡 =PMT(rate/12, nper*12, -pv) - **So i can have a positive number**

## Total Cost of Loan

- This one, I figured it out.
    - EMI * Nper*12

## Total Interest Amount

- Now we take the Loan amount and subtract the Total Cost of the Loan. I used the ABS formula to give me a positive number.
    - ABS(Loan Amount - Total Cost of Loan)

# Final results and summary

---

So the final result was this:

- According to the premise, Mr.Hathodwala’s monthly budget was 25000
- The results show that:

- ![Loan_Final_Result](https://github.com/Amjad-ali1997/Excel-Loan-Payment-Projection/assets/108399313/596917a7-7f67-4695-b2be-b80524aff6cd)
