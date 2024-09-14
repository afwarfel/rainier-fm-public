# Rainier Financial Model API

[API Documentation](https://rainierfm.com/docs)

Welcome to the landing page for my API. Here you can find information about the available endpoints and how to use them. This API is designed to let users interact with a financial model that I have built. My name is [Alex Warfel](https://www.linkedin.com/in/alexwarfel/). I earned my CFA charter in 2022 and have worked in the financial services industry, focusing on portfolio reporting, quantitative research, and technology solutions.

## Purpose

Determining how much money you should be saving to meet your life goals can be a daunting task. I began developing this financial model in 2017 to address this challenge, and I have been continuously refining and enhancing it ever since. The primary aim of this model is to assist individuals in understanding how much they need to save to achieve their financial objectives.

Traditional financial planning methods often rely on complex calculations such as net present value analysis or personal balance sheet evaluations, which can sometimes oversimplify the reality of one's financial situation. In contrast, this model employs a Monte Carlo simulation, which allows you to input various aspects of your financial circumstances. This approach provides a more nuanced and accurate determination of your optimal savings rate.

I would be immensely grateful if you could give this model a try. Your feedback is crucial in helping me further improve and fine-tune the model. There are numerous powerful insights that this model can offer. Below, you will find some examples of what the model can reveal, based on the inputs provided.

### Understand How Much You Should Be Saving Today to Achieve Your Goals

[View Interactive Chart](https://datawrapper.dwcdn.net/sUUdh/1/)

Above, you can see the results of a model run that estimates your optimal savings rate based on your goals, earnings, and other financial factors. The red areas highlight the savings rates that are most likely to help you achieve your financial objectives. This visualization provides a clear and intuitive way to understand how different savings rates can impact your ability to meet your goals. By analyzing these results, you can make more informed decisions about your savings strategy.

### Learn How Your Investments Are Likely to Change Over Your Lifetime

[View Interactive Chart](https://datawrapper.dwcdn.net/zXOPH/1/)

The chart above illustrates how your investments might evolve over your lifetime, particularly as you allocate funds towards achieving your goals. This visualization helps you understand the potential growth of your investments and the impact of your spending decisions on your financial future. By examining these projections, you can gain valuable insights into how different financial strategies may affect your long-term wealth.

### Understand What Your Future Potential Earnings Look Like

[View Interactive Chart](https://datawrapper.dwcdn.net/6SO9n/1/)

The results above were all created by passing in these variables below.

```javascript
modelInputs = {
    gross_current_income: 40000,
    gross_current_savings_rate: 0.25,
    assets: 2000,
    savings: 1000,
    tax_rate: 0.23,
    birthday: "2001-09-16 00:00:00",
    current_debt_accounts: {
        1: {
            balance: 5000,
            interest_rate: 0.05,
            minimum_payment: 100,
            name: "Credit Card"
        },
        2: {
            balance: 90000,
            interest_rate: 0.06,
            minimum_payment: 200,
            name: "Student Loan"
        },
        3: {
            balance: 10000,
            interest_rate: 0.04,
            minimum_payment: 100,
            name: "Car Loan"
        }
    },
    gender: "M",
    percentage_of_nominal_spending_for_housing: 0.25,
    initial_retirement_age: 65,
    non_retirement_goals: {
        1: {
            age: 35,
            amount_in_real_terms: 30000,
            chance_of_success: 0.75,
            name: "10k/year for beachhouse"
        }
    }
};
```

You can find the documentation for the financial model API here: [API Documentation](https://rainierfm.com/docs). There are several tools available to help you interact with the model. One of the most useful tools is [Postman](https://www.postman.com/downloads/). After downloading Postman, you can import the [Swagger JSON](https://rainierfm.com/swagger.json) from the provided link, and Postman will automatically integrate the API's details.

Models typically take about two minutes to run, and the results are stored in a database. You can access these results using your username and password. This ensures that you can review your model outputs at any time. If you encounter any issues or have questions, please feel free to contact me. Your feedback and inquiries are always welcome.

## Security

This API is secured by a third-party authentication service, ensuring that access is tightly controlled and monitored. Importantly, personally identifiable information (PII) is not stored in any of the databases used to power this API. In the unlikely event that our database is compromised, there is no information that links financial data to PII such as names or email addresses. Additionally, users have the ability to delete their PII at any time using one of the endpoints listed in the documentation, providing an extra layer of control and security.

## Methodology

The model employs Monte Carlo simulation, a robust statistical technique, to generate various financial scenarios. It innovatively creates time series for key variables such as interest rates, market returns, income growth, and change rates, as well as other path-dependent variables. The model also incorporates mortality rates and adjusts for changing housing costs, providing a comprehensive and realistic projection of financial outcomes. This methodology ensures that the model accounts for a wide range of factors that can influence financial planning.

---

© 2024 Rainier Financial Model. All rights reserved.

## Additional Information

- **API Location:** [https://rainierfm.com](https://rainierfm.com)
- **API Documentation:** [https://rainierfm.com/docs](https://rainierfm.com/docs)

---

**Note:** The interactive charts referenced above are available through the provided links. For the best experience, please view them in a web browser.

If you're interested in contributing to the project or have suggestions, please visit the [GitHub repository](#) (replace `#` with the actual repository link if available).