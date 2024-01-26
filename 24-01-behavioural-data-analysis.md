---
title: "Notes on behavioural data analysis"
author: "Chiawei Wang"
date: "January 2024"
---

`This document compiles information from Behavioral Data Analysis with R and Python for academic purposes`[^1]

[^1]: Buisson, Florent. 2021. *Behavioral Data Analysis with R and Python: Customer-Driven Data for Real Business Results*. O'Reilly: Sebastopol, California.

## The causal-behavioral framework for data analysis

Understanding what drives behaviors in order to change them is one of the key goals of applied analytics, whether in a business, a nonprofit, or a public organization. We want to figure out why someone bought something and why someone else didn’t buy it. We want to understand why someone renewed their subscription, contacted a call center instead of paying online, registered to be an organ donor, or gave to a nonprofit. Having this knowledge allows us to predict what people will do under different scenarios and helps us to determine what our organization can do to encourage them to do it again or not.

![Causal-behavioural framework for data analysis](https://github.com/x-square/visual-resources/blob/main/cause-behaviour-data.png?raw=true "Causal-behavioural framework for data analysis")

### Why we need causal analytics to explain human behavior?

Understanding where causal analytics fits into the analytics landscape will help us better identify why it is needed in business settings. As we’ll see, that need stems from the complexity of human behavior.

#### The different types of analytics

- **Descriptive analytics** provides a description of data. In simple terms, I think of it as **what is** or **what we've measured** analytics. Business reporting falls under that umbrella. How many customers canceled their subscriptions last month? How much profit did we make last year? Whenever we're calculating an average or other simple metrics, we’re implicitly using descriptive analytics.
- **Predictive analytics** provides a prediction. I think of it as **what will be, assuming current conditions persist** or **what we haven't yet measured** analytics. Most machine learning methods belong to this type of analytics and help us answer questions like **How many customers will cancel their subscription next month?** and **Is that order fraudulent?**
- **Causal analytics** provides the causes of data. I think of it as **what if?** or **what will be, under different conditions** analytics. It answers questions such as **How many customers will cancel their subscription next month unless we send them a coupon?** The most well-known tool of causal analytics is the A/B test, a.k.a. a randomized experiment or randomized controlled trial. That's because the simplest and most effective way to answer the preceding question is to send a coupon to a randomly selected group of customers and see how many of them cancel their subscription compared to a control group.

#### Human beings are complicated

If predictive analytics has been so successful and causal analytics uses the same data analysis tools like regression, why not stick with predictive analytics? In short, because human beings are more complicated than wind turbines. Human behavior:

- Has multiple causes
- Is context-dependent
- Is variable
- Is innovative
- Is strategic

### Confound It! The hidden dangers of letting regression sort it out

A regression for predictive analytics is used to estimate an unknown value (often, but not always, in the future). It does this by taking known information and using a variety of factors to triangulate the best guess value for a given variable. What is important is the predicted value and its accuracy, not why or how it was predicted.

Causal analytics also uses regression, but the focus is not on estimating a value of the target variable. Instead, the focus is on the cause of that value. In regression terms, our interest is no longer in the dependent variable itself but in its relationship with a given independent variable. With a correctly structured regression, the coefficient of correlation can be a portable measure of the causal effect of an independent variable on a dependent variable.

#### Berkson's paradox

If one of your customers has a strong taste for vanilla, this completely explains why they are shopping at your stand, and they don’t need to have a strong taste for chocolate. On the other hand, if one of your customers has a weak taste for vanilla, this can't explain why they are shopping at your stand, and they must have a stronger than average taste for chocolate.

The Berkson's paradox is counterintuitive and hard to understand at first. It can cause biases in your data, depending on how it was collected, even before you start any analysis.

## Understanding behavioral data

### Types of customer data

- **Demographic data** is information about your customers, like their age, gender, income, and education. It helps you know who your customers are and what they need. You can use this data to group your customers for marketing. For instance, if you sell anti-wrinkle cream, you might concentrate on age groups that are more likely to buy it. Gathering this data makes your marketing more focused and improves the outcomes.
- **Psychographic data** includes a customer's values, personality traits, opinions, attitudes, beliefs, and lifestyle. It goes beyond just demographic information. While demographics appeal to the logical side, psychographic data helps tap into the emotional aspect of buying decisions. Businesses and products don't have emotions, but humans do. Understanding what motivates your customer emotionally, what messaging resonates with them, and what brand attitude connects with them, becomes clearer with psychographic data. It's about making customers feel something to drive their buying decisions.
- **Behavioural data** includes customer actions, like purchases, website visits, or signing up for newsletters. It helps you grasp what your customers want and how they engage with your business. For instance, in the wrinkle cream case, if users of a certain age visit your website, click on product pages, and later sign up for your newsletter, it shows brand awareness and buyer intent. Analysing such data helps optimize touch points in your customer journey. Understanding when and why customers act the way they do enhances your marketing efforts, especially in re-engaging returning customers.
- **Transactional data** is details about a customer's financial activities, like how much they spend, how often they make purchases, the time it takes for them to buy, and how many items they return. This data helps marketers grasp spending habits and trends among customers, which becomes crucial when market conditions change, new technology emerges, or new factors affect buying decisions.

### How information acquired?

- **Theoretical approach** refers to information or predictions that are derived from theoretical principles, models, or hypotheses. This type of data is based on conceptual frameworks, ideas, or assumptions rather than direct observation or experimentation. Theoretical data often involves predictions or expectations about how a system or phenomenon should behave according to a given theoretical perspective. It serves as a foundation for designing experiments or conducting research.
- **Empirical approach**, on the other hand, is information that is obtained through direct observation, experimentation, or experience. This data is collected from real-world observations and measurements. It is tangible, verifiable, and based on evidence gathered through sensory experience or documented facts. Empirical data is crucial in scientific research as it provides the foundation for testing hypotheses, validating theories, and drawing conclusions based on observable phenomena.

### A basic model of human behavior

![Model of human behaviour for a midlife crisis](https://github.com/x-square/visual-resources/blob/main/human-behaviour-midlife-crisis.png?raw=true "Model of human behaviour for a midlife crisis")

![Model of human behaviour](https://github.com/x-square/visual-resources/blob/main/human-behaviour.png?raw=true "Model of human behaviour")

- Personal characteristics
    - Age, gender, family situation -- widely available and used
    - Personality traits, lifestyle habits e.g. a high degree of openness to experience and is always game to try some new flavor combination like blueberry and cheese
- Cognition and emotions -- collected through surveys (online or offline) or during user experience observation
    - Thoughts, mental models, beliefs
    - Customer satisfaction
- Intentions -- collected through surveys (online or offline) or during user experience observation
    - Mental states e.g. I'm going to book a vacation
    - Intent modeling
- Actions[^2] - the largest category of available customer data under transactional data
    - Basic unit of behavior e.g. going to the gym
- Business behaviors - what organization or its employees do that affect a customer
    - Communications e.g. modify the frequency and content of emails
    - Changes to website e.g. design, language
    - Business rules e.g. customer rewards
    - Decisions by employees e.g. labeling a customer account as potentially fraudulent or promoting another employee

[^2]: Note that the terms action and behaviour are often used interchangeably.

#### Personal characteristics

As a behavioral science mantra puts it, **behavior is a function of the person and the environment**, and social factors often have arguably more weight than demographic variables.

#### Cognition and emotions

One of the biggest differences between user experience or human-centered design and behavioral science is that **user experience begins with the presumption that human beings know what they want, how they feel about something and why**, whereas **behavioral science begins with the presumption that we are unaware of a lot of things going on in our own heads**.

To use a legal metaphor, a behavioral scientist will often treat what someone says as **suspicious until proven trustworthy**, whereas a user experience researcher will treat it as **honest until proven misleading**.

However, the distinction often gets blurred in practice, depending on the situation at hand. If a behavioral scientist is told by a customer that a website is confusing and frustrating to use, they will take a page from the user experience book and trust that the customer did indeed experience negative emotions. Conversely, when doing foundational product research, a skilled user experience researcher will often go beyond stated intentions and attempt to identify a customer's deeper needs.

#### Intentions

People often fail to follow through on things they want to do, a concept known in behavioral science as the **intention-action gap**. As an example, think of New Year's resolutions and how often they are broken.

Therefore, a key to driving customer behavior is determining whether a potential response doesn't occur because the customers don't want to take that action or because something happens between intention and action.

#### Actions

An action or behavior is something you should be able to observe if you were in the room at that moment without having to ask the person. **Buying something on Amazon** is an action. So is **reading a review of a product on Amazon**.

But **knowing something** or **deciding to buy something on Amazon** is not. You can't know that someone has made a decision unless you either ask them or see them acting on that decision which is a consequence but not the same thing.

#### Business behaviors

Business behaviors can be an analyst’s worst nightmare: like water to fish, they can be invisible to an organization, and their effects on individual behaviors then become intractable noise:

- First, many organizations, if they track business behaviors at all, simply don’t track them at the same level of detail as customer behaviors.
- Second, business behaviors can affect the interpretation of variables for customer behaviors. The clearest example of that would be sludges, intentional frictions and misleading communication introduced to confuse customers.

### How to connect behaviors and data?

Connecting behaviors and data is not simply a matter of assigning the variables at hand to one of these buckets. Being about behaviors is not enough for a variable to qualify as behavioral data as we saw in the previous section, for instance, a variable supposedly about customer behavior may really only reflect a business rule.

In this section, I'll give you a list of tips to behavioralize your data and ensure that it fits as closely as possible the qualitative reality it's supposed to represent.

- Develop a behaviroal integrity mindest
- Distrust and verify
- Identify data category
    - Personal characteristics
    - Cognition and emotions
    - Intentions
    - Actions
    - Business behaviors
- Refine behavioral variables
    - Observable e.g. you see customers do it
    - Individual e.g. if a variable makes sense only in the aggregate and doesn't have a meaningful interpretation at the individual level, that’s a red flag
    - Atomic e.g. a variety of different behaviors sharing a common intent
- Understand the context
    - It's about time e.g. frequency, duration, contiguity (doing X before doing Y), social schedules
    - Information and known unknowns
    - The dog that didn't bark e.g. what people don't do can often be as interesting as what they do

Often the best way to understand the context in which people behave is through qualitative research such as interviews and surveys, whose insights can be used to generate new variables.

## Introduction to causal diagrams

### Causal diagrams and the causal-behavioral framework

A causal diagram is a visual representation of variables, shown as boxes, and their relationships to each other shown as arrows going from one box to another.

Each rectangle represents a variable we can observe, and the arrow between them represents the existence and direction of a causal relationship.

Sometimes, however, there will be an additional variable that we aren’t able to observe. If we still want to show it in a causal diagram, we can represent it with a shaded rectangle.

![Example of causal diagram with unobserved variable](https://github.com/x-square/visual-resources/blob/main/causal-diagram.png?raw=true "Example of causal diagram with unobserved variable")

#### Causal diagrams represent behaviors

We intuitively understand that human beings have habits, preferences, and emotions, and we treat these as causes even though we often don't have any numeric data about them. When we say, **Joe bought peanuts because he was hungry**, we are relying on our knowledge, experience, and beliefs about humans in general and Joe in particular. We treat hunger as a real thing, even if we're not measuring Joe's blood sugar or brain activation.

Here, we're making a causal statement about reality: we're saying that **had Joe not been hungry, he wouldn't have bought peanuts**. Causality is so fundamental to our intuitive understanding of reality that even young children are able to make correct causal inferences evidenced by their use of the word **because** long before they have had any exposure to the scientific method or data analysis. Of course, intuition is subject to a variety of biases well known by behavioral scientists, even when it takes the more educated form of common sense or expertise. But more often than not, intuition guides us well in our daily lives even in the absence of quantitative data.

This subjectivity might look like a possibly fatal flaw of causal diagrams, but it’s actually a feature, not a bug. Causal diagrams don't create uncertainty; they simply reflect the uncertainty that is already in our world. If there are several possible interpretations of the situation at hand that appear equally valid, you should explicitly say so. The alternative would be to allow people who have different mental models in their heads to each believe that they know the truth and others agree with them, when in reality that’s not the case. At least putting the uncertainty in the open will allow a principled discussion and guide your analysis.

#### Causal diagrams represent data

When relationships between variables in our data are entirely linear, or approximately so, causal diagrams have clear equivalents in linear algebra. This means we can use the rules and tools of linear algebra to validate the **legality** of how we manipulate and transform causal diagrams, thus ensuring that we draw correct conclusions

The linearity requirement may seem very restrictive. However, some of the rules and tools of linear algebra continue to apply when some of these relationships are not linear but still belong to the broad category of models called generalized linear models. A **logistic regression** model for example is a generalized linear model. This means that we can represent and handle a causal relationship where the effect (depentant) variable is binary (**yes or no**) with causal diagrams. As the sidebar shows, the math gets more convoluted in that case, but most of our intuitions about causal diagrams remain true.

![Example of causal diagram of binary variables](https://github.com/x-square/visual-resources/blob/main/causal-diagram-binary-variables.png?raw=true "Example of causal diagram of binary variables")

### Fundamental structures of causal diagrams

- Chains
- Forks
- Colliders

Forks are also typical of situations where we look at demographic variables: age, gender, and place of residence all cause a variety of other variables that may or may not cause each other. You can picture a demographic variable such as age as being at the root of a fork with many teeth.

![Example of causal diagram of a chain](https://github.com/x-square/visual-resources/blob/main/causal-diagram-chain.png?raw=true "Example of causal diagram of a chain")

![Example of causal diagram of a fork](https://github.com/x-square/visual-resources/blob/main/causal-diagram-fork.png?raw=true "Example of causal diagram of a fork")

![Example of causal diagram of fork with a chain](https://github.com/x-square/visual-resources/blob/main/causal-diagram-fork-chain.png?raw=true "Example of causal diagram of fork with a chain")

![Example of causal diagram of a collider](https://github.com/x-square/visual-resources/blob/main/causal-diagram-collider.png?raw=true "Example of causal diagram of a collider")

![Example of causal diagram of a collider](https://github.com/x-square/visual-resources/blob/main/causal-diagram-collider.png?raw=true "Example of causal diagram of a collider")

![Example of causal diagram of three variables](https://github.com/x-square/visual-resources/blob/main/causal-diagram-three-variables.png?raw=true "Example of causal diagram of three variables")

### Common transformations of causal diagrams

Causal diagrams can be **collapsed** or **expanded** to focus on specific relations, direct or indirect.

Variables can themselves be sliced or aggregated to zoom in and out of specific behaviors and categories.

- **Slicing variables** means splitting a variable into sub variables e.g. from iced coffee sales to iced American sales and iced latte sales.
- **Aggregating variables** means merging more two or more relevant variables into a theme as a bigger variable e.g. from age and gender to demographics characteristics.

#### Cycles and paths

In real life, we often see variables that influence each other causally. This type of causal diagram is called a cycle. Cycles can arise for a variety of reasons. Two of the most common in behavioral data analysis are substitution effects and feedback loops. Fortunately, there are some workarounds that will allow you to deal with cycles when you encounter them.

- **Substitution effect** is a cornerstone of economics theory. Customers might substitute a product for another, depending on the products' availability and price and the customers' desire for variety e.g. customers choose between iced coffee and hot coffee based not only on temperature but also on special promotions and how often they had coffee this week.
- Another common cycle is a **feedback loop**, where a person modifies their behavior in reaction to changes in the environment e.g. a store manager keeps an eye on the length of waiting lines and open new lines if the existing ones get too long, so that customers don't give up and just leave.

![Example of causal diagram of substitution effect](https://github.com/x-square/visual-resources/blob/main/causal-diagram-substitution.png?raw=true "Example of causal diagram of substitution effect")

![Example of causal diagram of feedback loop](https://github.com/x-square/visual-resources/blob/main/causal-diagram-feedback-loop.png?raw=true "Example of causal diagram of feedback loop")

In almost all cases, it takes some **time** for one variable to influence another, which means you can **break the cycle** and turn it into an **acyclical** causal diagram e.g. it takes 15 minutes for a store manager to react to an increasing waiting time by getting new lines open, and it similarly takes 15 minutes for customers to adjust their perception of waiting time. In that case, by clarifying the temporal order of things, we can split the waiting time variable in our causal diagram.

![Example of causal diagram of time increments](https://github.com/x-square/visual-resources/blob/main/causal-diagram-time-increments.png?raw=true "Example of causal diagram of time increments")

Having seen the various ways variables can interact, we can now introduce one last concept, **paths**, which encompasses all of them. We say that there is a path between two variables **if there are arrows between them, regardless of the direction of the arrows, and if no variable appears twice along the way**.

## Building causal diagrams from scratch

Our goal in this book is always to measure the impact of one variable on another, which we can represent as a **starter** causal diagram as follows.

![The simplest possible causal diagram](https://github.com/x-square/visual-resources/blob/main/causal-diagram-simplest.png?raw=true "The simplest possible causal diagram")

### Business problem and data setup

- Understanding the relationship of interest

![Example of causal diagram of causal relationship of interest](https://github.com/x-square/visual-resources/blob/main/causal-diagram-relationship-interest.png?raw=true "Example of causal diagram of causal relationship of interest")

### Identify candidate variables to include

- Personal characteristics
- Cognition and emotions
- Intentions
- Actions
- Business behaviors
- Time trends

![Example of updated causal diagram at the final step](https://github.com/x-square/visual-resources/blob/main/causal-diagram-final-step.png?raw=true "Example of updated causal diagram at the final step")

### Validate observable variables to include based on data

- Relationships between numeric variables
- Relationships between categorical variables
- Relationships between numeric and categorical variables

![Observable variables between categorical and numeric](https://github.com/x-square/visual-resources/blob/main/causal-diagram-observable.png?raw=true "Observable variables between categorical and numeric")

![Correlation matrix for numeric and binary variables](https://github.com/x-square/visual-resources/blob/main/correlation-matrix-numeric-binary.png?raw=true "Correlation matrix for numeric and binary variables")

![Updated causal diagram of numeric and binary variables](https://github.com/x-square/visual-resources/blob/main/causal-diagram-numeric-updated.png?raw=true "Updated causal diagram of numeric and binary variables")

![Correlation matrix for categorical and binary variables](https://github.com/x-square/visual-resources/blob/main/correlation-matrix-categorical-binary.png?raw=true "Correlation matrix for categorical and binary variables")

![Updated causal diagram of categorical and binary variables](https://github.com/x-square/visual-resources/blob/main/causal-diagram-categorical-updated.png?raw=true "Updated causal diagram of categorical and binary variables")

Measuring correlations between numeric and categorical variables is a more cumbersome process than measuring correlations within a homogenous category. We can check if this is the case by comparing the mean of the numeric variable across the categories of the categorical variable. For example, we expect that the financial characteristics of the customer may impact the average daily rate for the reservation. Note that it would be best to explore that relationship after having built better variables for customer segmentation.

![Latest version of causal diagram of observable variables](https://github.com/x-square/visual-resources/blob/main/causal-diagram-observable-latest.png?raw=true "Latest version of causal diagram of observable variables")

### Expand Causal Diagram Iteratively

![Tentative causal diagram with unobservable variables](https://github.com/x-square/visual-resources/blob/main/causal-diagram-unobservable.png?raw=true "Tentative causal diagram with unobservable variables")

- Identify proxies for unobserved variables
- Identify further causes
- Iterate
- Simplify causal diagram to meet the need of the business
    - Collapse chains when the intermediary variables are not of interest or are unobserved.
    - Expand chains when you need to find observed variables or if you want to track the way another variable relates to the diagram.
    - Slice variables when you think the individual variables would contain interesting information (e.g. the correlation with one of your variables of interest is really driven by only one slice in particular).
    - Combine variables for clarity when reading the diagram or when variation between types does not matter.
    - Break cycles wherever you find them by introducing intermediary steps or identifying the aspect of the relationship that is important.

Unobserved variables represent a challenge, because even if they are confirmed through interviews or user research, they can't be accounted for directly in the regression analysis. We can still try to mitigate them somewhat by identifying potential proxies. For example, we may find that conscientiousness is indeed correlated with a lower rate of cancellation, but also with requesting a confirmation email.

Of course, requesting a confirmation email is not caused only by conscientiousness. It may also reflect the seriousness of the intent, lack of ease with digital channels, etc. And conversely, it may reduce the cancellation rate by itself, by providing easily accessible information on the reservation. Regardless, if we find that this behavior is negatively correlated with cancellation rate, we may leverage that insight by, for example, sending an SMS reminder to customers who didn’t choose to receive a confirmation email.

By brainstorming and validating through research potential proxies for unobserved variables, we're providing meaningful connections between observable variables. Knowing that requested confirmation is connected with cancellation through Conscientiousness provides a behavioral rationale for what would otherwise be a raw statistical regularity.

![Identify proxies for unobserved variables](https://github.com/x-square/visual-resources/blob/main/causal-diagram-proxies.png?raw=true "Identify proxies for unobserved variables")

There are however significant decreasing returns to this process. As you expand your causal diagram **outward**, the newly added variables will tend to have smaller and smaller correlations with your variables of interest, because of all the noise along the way. This means that accounting for them will deconfound your relationship of interest in smaller and smaller quantities.

The only observable variable without any parent (observable or unobservable) is Year, and obviously it can't have one (apart maybe from the laws of physics?), so this step doesn't apply.

![Simplified version of causal diagram](https://github.com/x-square/visual-resources/blob/main/causal-diagram-simplified.png?raw=true "Simplified version of causal diagram")

If this process seems long and somewhat tedious, that's because it is. Fortunately, this process is extremely cumulative and transferable. Once you've done it for a certain analysis, your knowledge of the causal relationships that matter for your business can be reused for another analysis.

Similarly, once someone has gone through the process, a new team member or employee can very easily and quickly acquire the corresponding knowledge and pick up where they left off by looking at the resulting causal diagram or even just the list of relevant variables to keep in mind.

## Using causal diagrams to deconfound data analyses

![Causal diagram for a business problem](https://github.com/x-square/visual-resources/blob/main/causal-diagram-business.png?raw=true "Causal diagram for a business problem")

![Causal diagram for the breakdown of a business problem](https://github.com/x-square/visual-resources/blob/main/causal-diagram-business-breakdown.png?raw=true "Causal diagram for the breakdown of a business problem")

In the upper left corner of the causal diagram, store staff has been instructed to offer the **Would you like spring water with that?** prompt both for sales of ice cream and for sales of French fries, on top of the **Would you like fries with that?** prompt for the sales of burgers.

In the bottom right corner of the causal diagram, the average age of customers (younger customers, and customers with children, are more likely to purchase sugary products) and the health mindset of customers (health-minded customers are more likely to buy water and less likely to buy sodas, everything else being equal).

### Disjunctive cause criterion

- First block
    - Include all variables that are a direct cause of both or either of our variables of interest e,g, number of customers that lead to ice cream sales and French fries sales that lead to bottled water sales
    - Exclude mediators between them e.g. anything between ice cream sales and bottled water sales in this case
    - Remove any confounding of our relationship of interest

![Causal diagram of collapsing confounders](https://github.com/x-square/visual-resources/blob/main/causal-diagram-collpaing-confounders.png?raw=true "Causal diagram of collapsing confounders")

- Second block
    - Include average age of store customers and health mindset of store customers
    - Exclude soda sales as it is not a cause of either ice cream sales or bottled water sales, but the problem is we don't have data for them yet

### Backdoor criterion

Definition

:   The causal relationship between two variables is confounded if there is at least one unblocked noncausal path between them starting with an arrow to our cause of interest. Conversely, to remove all confounding, we need to block all noncausal paths between them starting with an arrow to our cause of interest.

![A confounder is a joint cause and can be hidden](https://github.com/x-square/visual-resources/blob/main/confounder.png?raw=true "A confounder is a joint cause and can be hidden")

A path is causal if it's a chain. On the other hand, the path is noncausal because it includes at least one collider or fork.

## Handling missing data

- **Missing completely at random** occurs when the probability of missing data is unrelated to both observed and unobserved data. In simpler terms, the missing data happens randomly.
- **Missing at random** indicates the probability of missing data depends on the observed data but not on the unobserved data. The missing data is systematically related to the available information.
- **Missing not at random** means the probability of missing data is related to the unobserved data even after considering the observed data. This type of missing data introduces potential biases as it's not random.
- **Multiple imputation** fills in missing values by generating plausible numbers derived from distributions of and relationships among observed variables in the data set.
- **Predictive mean matching** aims to reduce the bias introduced in a dataset through imputation, by drawing real values sampled from the data. This is achieved by building a small subset of observations where the outcome variable matches the outcome of the observations with missing values.
- **Auxiliary variables** are additional variables included in statistical models to improve precision, handle missing data, or control for potential confounding factors. They are not the main focus of the analysis but provide valuable information to enhance the accuracy and reliability of parameter estimates.

![Decision tree to diagnose missing data](https://github.com/x-square/visual-resources/blob/main/decision-tree-missing-data.png?raw=true "Decision tree to diagnose missing data")

## Measuring uncertainty with the bootstrap

- **Bootstrapping** is a resampling technique used in statistics to help us figure out how confident we can be in our results, even when our data is limited or a bit messy. Instead of making assumptions about data we didn't collect, we use the information we do have to create many imaginary datasets. This lets us calculate things like confidence intervals and errors, giving us a better understanding of how sure we can be about our findings.
- **Influential points** are data observations with a big impact on results, like in regression models. They strongly affect estimated values and the model's overall fit. These points usually have extreme values or unusual patterns that greatly impact statistical outcomes. Spotting and handling them is vital for a strong and reliable statistical analysis.
- **Cook's distance** is a statistical measure used in regression analysis to assess the influence of individual data points on the overall fit of the model. It helps identify influential observations that can significantly affect the regression coefficients and predictions. High Cook's distance values suggest that removing the corresponding data point could have a substantial impact on the model. Analysts often use Cook's distance to detect outliers and assess the robustness of their regression models.
- **Regression residuals** are the differences between the actual values of the dependent variable and the values predicted by the regression model. They capture how much each data point deviates or resides away from the model's predictions. By examining these residuals, analysts can assess how well the model fits the data. If the residuals show a systematic pattern or are consistently large, it suggests that the model may need refinement, and further investigation is needed to enhance its accuracy and effectiveness.
- **Density plot** is a graphical representation of the distribution of a continuous variable. It provides a smooth curve that estimates the probability density function of the data. The primary purpose of a density plot is to visualize the underlying distribution of a dataset, allowing you to see patterns, peaks, and gaps in the data.
- **Quantile-quantile plot** is a graphical tool used to assess whether a dataset conforms to a specific theoretical distribution, such as the normal distribution. It compares the quantiles of the observed data to the quantiles expected from the theoretical distribution. If the points on the plot fall along a straight line, it suggests a good fit with the chosen distribution. Deviations from the line indicate potential departures from the assumed distribution, providing insights into the characteristics of the dataset.

![Decision tree to to use bootstrap](https://github.com/x-square/visual-resources/blob/main/decision-tree-bootstrap.png?raw=true "Decision tree to to use bootstrap")

Analysing behavioural data, especially if it's small or unusual, can be tricky. Luckily, the bootstrap method, aided by computer simulations, is a valuable tool. It helps handle uncertainties in estimates without relying on assumptions about data distribution. For observational data showing signs of outliers or non-normality, bootstrap is particularly useful. In experimental data, where decisions often rely on *p* values, the bootstrap method becomes crucial.

## Experimental design: The basics

- **Theory of change** is a framework commonly used in the field of behavioural science. It outlines the causal pathways through which interventions are expected to bring about desired outcomes. It helps organisations and researchers understand the logic behind their interventions and assess whether they are achieving the intended impact.
    - For example, implementing `intervention` through `behavioral logic` as measured by `target metric` will help us achieve `business goal`.
    - That is, implementing `one-click booking button` through `a reduction in the duraiton of the booking process` as measured by `booking probability` will help us achieve `higher revenue`.

![Example of theory of change](https://github.com/x-square/visual-resources/blob/main/theory-change.png?raw=true "Example of theory of change")

Normally, we approach the theory of change of our experiment backwards to ensure we address our business goals. That is, to boost revenue, we must increase completed bookings. This involves streamlining the booking process by introducing a one-click button at a suitable touchpoint. Our hypothesis is that customers leave because of the frustration caused by a lengthy, complex process.

> If I had an hour to solve a problem, I'd spend 55 minutes thinking about the problem and 5 minutes thinking about solutions, Albert Einstein.

- **Power analysis** is like figuring out how many people we need in our study to be sure we can find a real difference if it's there. It helps us make sure our research is strong enough to catch important things without making the mistake of saying there's no difference when there actually is. We think about things like how sure we want to be and how big the difference might be. This way, we plan our studies to be really good at finding important information.
- **Effect size** is a way to measure how big or strong a difference or relationship is in a study. It helps us understand the practical importance of our findings, regardless of the number of people in the study. Different measures like Cohen's d or correlation coefficients are used to express this size. Essentially, it gives us a clearer picture of the impact or significance of what we're studying.
- **Statistical power** is like the ability of a study to catch a real effect. If the power is high, close to 1, it's good at finding real things. If it's low that, close to 0, there's a risk of missing real effects. It depends on factors like the number of participants, the significance level, and the size of the effect being studied. Researchers want high power to make sure their studies are strong and can find meaningful results.
- **Sharp null hypothesis** is a specific and precise statement about a parameter in a statistical model. It typically posits that the parameter takes on a particular, exact value. For example, a sharp null hypothesis could state that the average score on a test for a certain group is exactly 75.
- **Composite null hypothesis** is more flexible. It allows for a range of values for the parameter. For instance, a composite null hypothesis might state that the average score on the test is equal to or less than 75, suggesting a broader set of possibilities.

`Any questions, please reach out`

Image via Behavioral Data Analysis with R and Python

Chiawei Wang, PhD\
Data Scientist\
<chw.wng@outlook.com>
