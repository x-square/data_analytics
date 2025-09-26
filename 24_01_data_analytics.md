---
title: 'Notes on Data Analytics'
author: 'Chiawei Wang'
date: 'January 2024'
---

`This document compiles information from Google Data Analytics for academic purposes.`[^1]

[^1]: [Google Data Analytics](https://www.coursera.org/professional-certificates/google-data-analytics 'Google professional certificate') includes over 180 hours of instruction and hundreds of practice-based assessments, which will help you simulate real-world data analytics scenarios that are critical for success in the workplace. The content is highly interactive and exclusively developed by Google employees with decades of experience in data analytics. Through a mix of videos, assessments, and hands-on labs, you'll get introduced to analysis tools and platforms and key analytical skills required for an entry-level job.

Data analytics is the collection, transformation and organization of data in order to draw conclusions, make predictions and drive informed decision making.

# Foundations of data analytics

## Thinking about analytical thinking

- **Curiosity**: a desire to know more about something, asking the right questions
- **Understanding context**: understanding where information fits into the **big picture**
- **Having a technical mindset**: breaking big things into smaller steps
- **Data design**: thinking about how to organize data and information
- **Data strategy**: thinking about the people, processes, and tools used in data analysis

## Variations of the data life cycle

The data life cycle provides a generic or common framework for how data is managed.

1. **Plan**: Decide what kind of data is needed, how it will be managed, and who will be responsible for it.
2. **Capture**: Collect or bring in data from a variety of different sources.
3. **Manage**: Care for and maintain the data. This includes determining how and where it is stored and the tools used to do so.
4. **Analyze**: Use the data to solve problems, make decisions, and support business goals.
5. **Archive**: Keep relevant data stored for long-term and future reference.
6. **Destroy**: Remove data from storage and delete any shared copies of the data.

## Six phases of data analysis

Analysts use data-driven decision-making and follow a step-by-step process:

1. **Ask** questions and define the problem
2. **Prepare** data by collecting and storing the information
3. **Process** data by cleaning and checking the information
4. **Analyze** data to find patterns, relationships and trends
5. **Share** data with your audience
6. **Act** on the data and use the analysis results

![Data analysis process](https://github.com/x-square/visual-resources/blob/main/data-analysis-process.png?raw=true 'Data analysis process')

## Structured query language

SQL (structured query language) is designed for managing and manipulating relational databases. It is used for tasks such as querying data, updating records, inserting new data and deleting information from databases.

- **SELECT** to choose the columns you want to return
- **FROM** to choose the tables where the columns you want are located
- **WHERE** to filter for certain information

![Example of SQL syntax](https://github.com/x-square/visual-resources/blob/main/sql-syntax.png?raw=true 'Example of SQL syntax')

BigQuery is Google's fully managed, serverless data warehouse that works across clouds and enables scalable analysis. It supports querying using a dialect of SQL.

> [!TIP]
> - \% is used as a wildcard to match one or more characters
> - \<\> means does not equal


## The power of data in business

- **Issue**
    - A topic or subject to investigate
- **Question**
    - Designer to discover information
- **Problem**
    - An obstacle or complication that needs to be worked out
- **Business task**
    - The question or problem data analysis answers for a business e.g. analyse weather data from the last decade to identify predictable patterns
- **Data-driven decision-making**
    - Using facts to guide bushiness strategy

## Exploring your next job

![Decoding job description for data professionals](https://github.com/x-square/visual-resources/blob/main/data-job-description.png?raw=true 'Decoding job description for data professionals')

# Ask questions to make data-driven decisions

## Solve problems with data

Data analytics is so much more than just plugging information into a platform to find insights. It is about solving problems. To get to the root of these problems and find practical solutions, there are lots of opportunities for creative thinking. No matter the problem, the first and most important step is understanding it.

![Analysts typically work with six problem types](https://github.com/x-square/visual-resources/blob/main/problem-types-six.png?raw=true 'Analysts typically work with six problem types')

Examples are summarized below for review:

### Making predictions

A company that wants to know the best advertising method to bring in new customers is an example of a problem requiring analysts to make predictions. Analysts with data on location, type of media, and number of new customers acquired as a result of past ads can't guarantee future results, but they can help predict the best placement of advertising to reach the target audience.

### Categorising things

An example of a problem requiring analysts to categorize things is a company's goal to improve customer satisfaction. Analysts might classify customer service calls based on certain keywords or scores. This could help identify top-performing customer service representatives or help correlate certain actions taken with higher customer satisfaction scores.

### Spotting something unusual

A company that sells smart watches that help people monitor their health would be interested in designing their software to spot something unusual. Analysts who have analyzed aggregated health data can help product developers determine the right algorithms to spot and set off alarms when certain data doesn't trend normally.

### Identifying themes

Designers often collaborate with analysts to analyze user interaction data. Analysts play a crucial role in categorising and identifying themes within the data, particularly in usability improvement projects. Themes, such as user beliefs, practices and needs, help researchers delve into specific aspects of the data, offering valuable insights for prioritising product features. While categorising involves assigning items to categories, identifying themes goes a step further, grouping categories into broader themes.

### Discovering connections

A third-party logistics company working with another company to get shipments delivered to customers on time is a problem requiring analysts to discover connections. By analyzing the wait times at shipping hubs, analysts can determine the appropriate schedule changes to increase the number of on-time deliveries.

### Finding patterns

Minimising downtime caused by machine failure is an example of a problem requiring analysts to find patterns in data. For example, by analyzing maintenance data, they might discover that most failures happen if regular maintenance is delayed by more than a 15-day window.

## SMART questions

Companies in lots of industries today are dealing with rapid change and rising uncertainty. Even well-established businesses are under pressure to keep up with what is new and figure out what is next. To do that, they need to ask questions. Asking the right questions can help spark the innovative ideas that so many businesses are hungry for these days.

No matter how much information you have or how advanced your tools are, your data won't tell you much if you don't start with the right questions. Think of it like a detective with tons of evidence who doesn't ask a key suspect about it.

![Examples of SMART questions](https://github.com/x-square/visual-resources/blob/main/smart-questions.png?raw=true 'Examples of SMART questions')

## Data trials and triumphs

### Coke launch failure

In 1985, New Coke was launched, replacing the classic Coke formula. The company had done taste tests with 200,000 people and found that test subjects preferred the taste of New Coke over Pepsi, which had become a tough competitor. Based on this data alone, classic Coke was taken off the market and replaced with New Coke. This was seen as the solution to take back the market share that had been lost to Pepsi.

But as it turns out, New Coke was a massive flop and the company ended up losing tens of millions of dollars. How could this have happened with data that seemed correct? It is because the data wasn't complete, which made it inaccurate. The data didn't consider how customers would feel about New Coke replacing classic Coke. The company's decision to retire classic Coke was a data-driven decision based on incomplete data.

### Mars orbiter loss

In 1999, NASA lost the \$125 million Mars Climate Orbiter, even though it had good data. The spacecraft burned to pieces because of poor collaboration and communication. The Orbiter's navigation team was using the SI or metric system (newtons) for their force calculations, but the engineers who built the spacecraft used the English Engineering Units system (pounds) for force calculations.

No one realized a problem even existed until the Orbiter burst into flames in the Martian atmosphere. Later, a NASA review board investigating the root cause of the problem figured out that the issue was isolated to the software that controlled the thrusters. One program calculated the thrusters' force in pounds; another program looking at the data assumed it was in newtons. The software controllers were making data-driven decisions to adjust the thrust based on 100% accurate data, but these decisions were wrong because of inaccurate assumptions when interpreting it. A conversion of the data from one system of measurement to the other could have prevented the loss. Note that the data-informed approach can be considered in this case.

> [!TIP]
> - **Data-inspired** approach (subjective) involves drawing inspiration and insights from data but doesn't necessarily dictate decisions. It acknowledges that data can provide valuable perspectives and ideas, serving as a source of inspiration for further exploration or consideration.
> - **Data-informed** approach (inter-subjective) plays a more significant role in decision-making. Decisions are influenced by data, which is used to guide and support the decision-making process. However, other factors, such as experience or intuition, may still be taken into account.
> - **Data-driven** approach (objective) places data at the forefront of decision-making. Decisions are primarily based on the analysis and interpretation of data. This approach emphasizes using data to measure outcomes, predict trends, and guide strategic choices. It often involves relying heavily on quantitative evidence to inform decisions.

## Qualitative and quantitative data in business

- **Qualitative data**
    - Subjective or explanatory measures of qualities and characteristics
- **Quantitative data**
    - Specific and objective measures of numerical facts

We can take a closer look at the data types and data collection tools. Imagine that you are a data analyst for a chain of movie theaters. Your manager wants you to track trends in:

- Movie attendance over time
- Profitability of the concession stand
- Evening audience preferences

In our scenario, we assume quantitative data already exists to monitor all three trends. Since we know that the movie theater is planning to raise ticket prices for evening showtimes in a few months, we will also include a question in the survey to get an idea of customers' price sensitivity.

Your final online survey might include these questions for qualitative data:

- What went into your decision to see a movie in our theater today? (movie attendance)
- What do you think about the quality and value of your purchases at the concession stand? (concession stand profitability)
- Which showtime do you prefer, 8:00 PM or 8:30 PM, and why do you prefer that time? (evening movie-goer preferences)
- Under what circumstances would you choose a matinee over a night time showing? (ticket price increase)

Data analysts will generally use both types of data in their work. Usually, qualitative data can help analysts better understand their quantitative data by providing a reason or more thorough explanation. In other words, quantitative data generally gives you the what, and qualitative data generally gives you the why. By using both quantitative and qualitative data, you can learn when people like to go to the movies and why they chose the theater. Maybe they really like the reclining chairs, so your manager can purchase more recliners. Maybe the theater is the only one that serves root beer. Maybe a later show time gives them more time to drive to the theater from where popular restaurants are located. Maybe they go to matinees because they have kids and want to save money. You wouldn't have discovered this information by analyzing only the quantitative data for attendance, profit, and showtimes.

## Connecting the data dots

When thinking about the benefits and challenges of big data, it helps to think about the four Vs:

| **Volume** | **Variety** | **Velocity** | **Veracity** |
|------------|-------------|--------------|--------------|
| Amount of data | Different kinds of data | How fast the data can be processed | Quality and reliability of the data |

: Four Vs for big data

## Structured thinking and scope of work

Structured thinking is the process of recognizing the currect problem or situation, organizing available information, revealing gaps and opportunities, and identifying the options.

Scope of work is an agreed-upon outline of the work you're going to perform on a project:

- **Deliverables** are items or tasks you will complete before you can finish the project.
- **Timelines** include due dates for when deliverables, milestones, and or reports are due.
- **Milestones** are significant tasks you will confirm along your timeline to help everyone know the project is on track.
- **Reports** notify everyone as you finalize deliverables and meet milestones.

![Example of scope of work](https://github.com/x-square/visual-resources/blob/main/scope-of-work.png?raw=true 'Example of scope of work')

![Example of scope of work in the spreadsheet](https://github.com/x-square/visual-resources/blob/main/scope-of-work-spreadsheet.png?raw=true 'Example of scope of work in the spreadsheet')

## Importance of context

Context is the condition in which something exists or happens. Context is important in data analytics because it helps us sift through huge amounts of disorganized data and turn it into something meaningful. The fact is, data has little value if it is not paired with context.

Context can turn raw data into meaningful information. It is very important for data analysts to contextualize their data. This means giving the data perspective by defining it. To do this, you need to identify:

- **Who** the person or organization that created, collected and or funded the data collection
- **What** the things in the world that data could have an impact on
- **Where** the origin of the data
- **When** the time when the data was created or collected
- **Why** the motivation behind the creation or collection
- **How** the method used to create or collect it

Here are some questions to help you get started:

- What is the problem?
- Can it be solved with data? If so, what data?
- Where is this data? Does it exist, or do you need to collect it?
- Are you using private data that someone will need to give you access to, or publicly available data?
- Who are the relevant sponsors and stakeholders for this project? Who is involved, and how?
- What are the boundaries for your project? What do you consider in-scope? What do you consider out-of-scope?
- Is there any other information you think is relevant to the project?
- Is there any information you need or questions you need answered before you can begin?

## Working with stakeholders

Your data analysis project should answer the business task and create opportunities for data-driven decision-making. That's why it is so important to focus on project stakeholders. As a data analyst, it is your responsibility to understand and manage your stakeholders' expectations while keeping the project goals front and center.

You might remember that stakeholders are people who have invested time, interest, and resources into the projects that you are working on. This can be a pretty broad group, and your project stakeholders may change from project to project. But there are three common stakeholder groups that you might find yourself working with: the executive team, the customer-facing team, and the data science team.

Let's get to know more about the different stakeholders and their goals. Then we'll learn some tips for communicating with them effectively.

### Executive team

The executive team provides strategic and operational leadership to the company. They set goals, develop strategy, and make sure that strategy is executed effectively. The executive team might include vice presidents, the chief marketing officer, and senior-level professionals who help plan and direct the company's work. These stakeholders think about decisions at a very high level and they are looking for the headline news about your project first. They are less interested in the details. Time is very limited with them, so make the most of it by leading your presentations with the answers to their questions. You can keep the more detailed information handy in your presentation appendix or your project documentation for them to dig into when they have more time.

For example, you might find yourself working with the vice president of human resources on an analysis project to understand the rate of employee absences. A marketing director might look to you for competitive analyses. Part of your job will be balancing what information they will need to make informed decisions with their busy schedule.

But you don't have to tackle that by yourself. Your project manager will be overseeing the progress of the entire team, and you will be giving them more regular updates than someone like the vice president of HR. They are able to give you what you need to move forward on a project, including getting approvals from the busy executive team. Working closely with your project manager can help you pinpoint the needs of the executive stakeholders for your project, so don't be afraid to ask them for guidance.

### Customer-facing team

The customer-facing team includes anyone in an organization who has some level of interaction with customers and potential customers. Typically they compile information, set expectations, and communicate customer feedback to other parts of the internal organization. These stakeholders have their own objectives and may come to you with specific asks. It is important to let the data tell the story and not be swayed by asks from your stakeholders to find certain patterns that might not exist.

Let's say a customer-facing team is working with you to build a new version of a company's most popular product. Part of your work might involve collecting and sharing data about consumers' buying behavior to help inform product features. Here, you want to be sure that your analysis and presentation focuses on what is actually in the data, not on what your stakeholders hope to find.

### Data science team

Organizing data within a company takes teamwork. There's a good chance you'll find yourself working with other data analysts, data scientists, and data engineers. For example, maybe you team up with a company's data science team to work on boosting company engagement to lower rates of employee turnover. In that case, you might look into the data on employee productivity, while another analyst looks at hiring data. Then you share those findings with the data scientist on your team, who uses them to predict how new processes could boost employee productivity and engagement. When you share what you found in your individual analyses, you uncover the bigger story. A big part of your job will be collaborating with other data team members to find new angles of the data to explore.

Here's a view of how different roles on a typical data science team support different functions:

![Data science team supports different functions](https://github.com/x-square/visual-resources/blob/main/data-science-cross-functions.png?raw=true 'Data science team supports different functions')

### Working effectively with stakeholders

When you're working with each group of stakeholders from the executive team, to the customer-facing team, to the data science team, you'll often have to go beyond the data. Use the following tips to communicate clearly, establish trust, and deliver your findings across groups.

#### Discuss goals

Stakeholder requests are often tied to a bigger project or goal. When they ask you for something, take the opportunity to learn more. Start a discussion. Ask about the kind of results the stakeholder wants. Sometimes, a quick chat about goals can help set expectations and plan the next steps.

#### Feel empowered to say no

When faced with urgent data analysis requests from a marketing director for a **high-priority project**, assess feasibility and push back if necessary. Stakeholders may not fully understand the time and effort involved, so clarify expectations by asking about their goals. Be confident in saying no if you can't meet the timeline, and guide them towards more realistic options. Prioritize effectively, communicate limitations, and empower stakeholders to reset expectations based on achievable timelines. Feel empowered to say **no**, but provide context for better understanding.

#### Plan for the unexpected

Before you start a project, make a list of potential roadblocks. Then, when you discuss project expectations and timelines with your stakeholders, give yourself some extra time for problem-solving at each stage of the process.

#### Know your project

Keep track of your discussions about the project over email or reports, and be ready to answer questions about how certain aspects are important for your organization. Get to know how your project connects to the rest of the company and get involved in providing the most insight possible. If you have a good understanding about why you are doing an analysis, it can help you connect your work with other goals and be more effective at solving larger problems.

#### Start with words and visuals

It is common for data analysts and stakeholders to interpret things in different ways while assuming the other is on the same page. This **illusion of agreement** shown as follows has been historically identified as a cause of projects going back-and-forth a number of times before a direction is finally nailed down. To help avoid this, start with a description and a quick visual of what you are trying to convey. Stakeholders have many points of view and may prefer to absorb information in words or pictures. Work with them to make changes and improvements from there. The faster everyone agrees, the faster you can perform the first analysis to test the usefulness of the project, measure the feedback, learn from the data, and implement changes.

#### Communicate often

Your stakeholders will want regular updates on your projects. Share notes about project milestones, setbacks, and changes. Then use your notes to create a shareable report. Another great resource to use is a change-log, which is a tool that will be explored further throughout the program. For now, just know that a is a file containing a chronologically ordered list of modifications made to a project. Depending on the way you set it up, stakeholders can even pop in and view updates whenever they want.

![Example of illusion of agreement via Typical Project Life](https://github.com/x-square/visual-resources/blob/main/typical-project-life.png?raw=true 'Example of illusion of agreement via Typical Project Life')

## Data scenarios and responses

When you communicate your analysis and recommendations as a data analyst, it's vital to keep your audience in mind. :

- Who is our audience?
    - Kiri, Product Development Project Manager
- What do they already know?
    - Kiri received updates about our project from its planning stages, including the most recent project report, sent two weeks ago.
- What do they need to know?
    - Kiri needs an update on the analysis project's progress and needs to know that the executive team approved changes to the data and timeline. You know that adding a new variable to the analysis will impact the current project timeline. Kiri will need to change the project's milestones and completion date.
- How can we best communicate what they need to know?
    - You can start by sending an email update to Kiri with the latest timeline for the project, but a meeting might be necessary if she wants to talk through her concerns about missing a deadline.

![Sample of updated timeline email](https://github.com/x-square/visual-resources/blob/main/email-timelime.png?raw=true 'Sample of updated timeline email')

![Sample of project follow-up email](https://github.com/x-square/visual-resources/blob/main/email-follow-up.png?raw=true 'Sample of project follow-up email')

## Limitations of data

Data is powerful, but it has its limitations. Has someone's personal opinion found its way into the numbers? Is your data telling the whole story? Part of being a great data analyst is knowing the limits of data and planning for them.

- Case of incomplete or non-existent data
    - If your data is incomplete or missing, you may realize during analysis that you lack sufficient information for a conclusion or may be addressing a different issue. For instance, if seeking employees with a specific certificate, but certification records only cover the last two years, you can still use the data, but highlight the analysis limitations. You could explore alternative data sources, like contacting the training company, but transparently communicate the incomplete dataset until additional data is obtained.
- Don't miss misaligned data
    - When collecting data from various teams and existing spreadsheets, be aware that different teams may apply distinct business rules. For instance, one team may define a metric based on all trainees who registered, while another team counts only those who completed the program. Standardizing measurement approaches early on ensures consistency, reliability, and accuracy in the data. This practice facilitates meaningful and insightful comparisons between teams.
- Deal with dirty data
    - Dirty data, containing errors, can result in productivity loss, unnecessary spending, and poor decision-making. Data cleaning, the process of fixing or removing incorrect, corrupted, and incomplete data, helps prevent these issues. Learning how to clean data is crucial to avoid data disasters, and this will be covered later in the training.
- Tell a clear story
    - Compare the same types of data
    - Visualize with care
    - Leave out needless graphs
    - Test for statistical significance
    - Pay attention to sample size
- Be the judge
    - In organizations, data analysts play a key role in making informed judgments. Understanding data limitations enables making decisions based on accurate information. Incomplete or uncleaned data can be misleading. Ensure data completeness and consistency by cleaning it before analysis, saving time and effort.

## Leading great meetings

![Example of meeting agenda](https://github.com/x-square/visual-resources/blob/main/meeting-agenda.png?raw=true 'Example of meeting agenda')

# Prepare data for exploration

## Selecting the right data

![How to collect the right data?](https://github.com/x-square/visual-resources/blob/main/data-collection-considerations.png?raw=true 'How to collect the right data?')

## Data formats in practice

| **Data Format Classification** | **Definition** | **Examples** |
| ------------------------------ | -------------- | ------------ |
| Primary data | Collected by a researcher from first-hand sources | <li> Data from an interview you conducted <li>Data from a survey returned from 20 participants <li> Data from questionnaires you got back from a group of workers |
| Secondary data | Gathered by other people or from other research | <li> Data you bought from a local data analytics firm's customer profiles <li> Demographic data collected by a university <li> Census data gathered by the federal government |
| Internal data | Data that lives inside a company's own systems | <li> Wages of employees across different business units tracked by HR <li> Sales data by store location <li> Product inventory levels across distribution centers |
| External data | Data that lives outside of a company or organization | <li> National average wages for the various positions throughout your organization <li> Credit reports for customers of an auto dealership |
| Continuous data | Data that is measured and can have almost any numeric value | <li> Height of kids in third grade classes (52.5 inches, 65.7 inches) <li> Runtime markers in a video <li> Temperature |
| Discrete data | Data that is counted and has a limited number of values| <li> Number of people who visit a hospital on a daily basis (10, 20, 200) <li> Room's maximum capacity allowed <li> Tickets sold in the current month |
| Qualitative | Subjective and explanatory measures of qualities and characteristics | <li> Exercise activity most enjoyed <li> Favorite brands of most loyal customers <li> Fashion preferences of young adults |
| Quantitative | Specific and objective measures of numerical facts | <li> Percentage of board certified doctors who are women <li> Population of elephants in Africa <li> Distance from Earth to Mars |
| Nominal | A type of qualitative data that isn't categorized with a set order | <li> First time customer, returning customer, regular customer <li> New job applicant, existing applicant, internal applicant <li> New listing, reduced price listing, foreclosure |
| Ordinal | A type of qualitative data with a set order or scale | <li> Movie ratings (number of stars: 1 star, 2 stars, 3 stars)  <li> Ranked-choice voting selections (1st, 2nd, 3rd) <li> Income level (low income, middle income, high income) |
| Structured data | Data organized in a certain format, like rows and columns | <li> Expense reports <li> Tax returns <li> Store inventory |
| Unstructured data | Data that isn't organized in any easily identifiable manner | <li> Social media posts <li> Emails <li> Videos |

: Data format examples

![Example of data formats](https://github.com/x-square/visual-resources/blob/main/data-formats.png?raw=true 'Example of data formats')

## Structure of data

Data is everywhere and it can be stored in lots of ways. Two general categories of data are:

- **Structured data**: Organized in a certain format, such as rows and columns
    - When you rate your favorite restaurant online, you're creating structured data.
    - This makes it easier to store and query for business needs. If the data is exported, the structure goes along with the data.
- **Unstructured data**: Not organized in any easy-to-identify way
    - When you use Google Earth to check out a satellite image of a restaurant location, you're using unstructured data.
    - There is much more unstructured than structured data in the world. Video and audio files, text files, social media content, satellite imagery, presentations, PDF files, open-ended survey responses, and websites all qualify as types of unstructured data.


![Structured and unstructured data](https://github.com/x-square/visual-resources/blob/main/data-structured-unstructured.png?raw=true 'Structured and unstructured data')

Data type definitions:

- **First-party data** is collected by an individual or group using their own resources and is often highly reliable.
- **Second-party data** is collected by a group directly from its audience and then sold.
- **Third-party data** can be less reliable because it comes from outside sources who did not collect it directly.

The lack of structure makes unstructured data difficult to search, manage, and analyze. But recent advancements in artificial intelligence and machine learning algorithms are beginning to change that.

### Fairness issue

Now, the new challenge facing data scientists is making sure these tools are inclusive and unbiased. Otherwise, certain elements of a dataset will be more heavily weighted and or represented than others. And as you're learning, an unfair dataset does not accurately represent the population, causing skewed outcomes, low accuracy levels, and unreliable analysis.

## Data modelling levels and techniques

Data models help keep data consistent and enable people to map out how data is organized. A basic understanding makes it easier for analysts and other stakeholders to make sense of their data and use it in the right ways.

**Data modelling** is the process of creating diagrams that visually represent how data is organized and structured. These visual representations are called **data models**. You can think of data modelling as a blueprint of a house. At any point, there might be electricians, carpenters, and plumbers using that blueprint. Each one of these builders has a different relationship to the blueprint, but they all need it to understand the overall structure of the house. Data models are similar. Different users might have different data needs, but the data model gives them an understanding of the structure as a whole.

### Levels of data modeling

- Conceptual data modeling gives a high-level view of the data structure, such as how data interacts across an organization. For example, a conceptual data model may be used to define the business requirements for a new database. A conceptual data model doesn't contain technical details.
- Logical data modeling focuses on the technical details of a database such as relationships, attributes, and entities. For example, a logical data model defines how individual records are uniquely identified in a database. But it doesn't spell out actual names of database tables. That's the job of a physical data model.
- Physical data modeling depicts how a database operates. A physical data model defines all entities and attributes used; for example, it includes table names, column names, and data types for the database.

![Common types of data modeling](https://github.com/x-square/visual-resources/blob/main/data-modeling.png?raw=true 'Common types of data modeling')

More information can be found in this [comparison of data models](https://www.1keydata.com/datawarehousing/data-modeling-levels.html).

### Data-modeling techniques

There are a lot of approaches when it comes to developing data models, but two common methods are the **Entity Relationship Diagram** (ERD) and the **Unified Modelling Language** (UML) diagram. ERDs are a visual way to understand the relationship between entities in the data model. UML diagrams are very detailed diagrams that describe the structure of a system by showing the system's entities, attributes, operations, and their relationships. As a junior data analyst, you will need to understand that there are different data modelling techniques, but in practice, you will probably be using your organization's existing technique.

![Example of ERD](https://github.com/x-square/visual-resources/blob/main/diagram-erd.png?raw=true 'Example of ERD')

![Example of UML](https://github.com/x-square/visual-resources/blob/main/diagram-uml.png?raw=true 'Example of UML')

## Understanding Boolean logic

Boolean logic is a type of algebra in which results are calculated as either **TRUE** or **FALSE**.

Boolean operators, similar to mathematical operators, help create logical statements. Data analysts use these statements for various tasks like crafting queries for searches and checking conditions in programming code during data analysis.

Imagine you are shopping for shoes, and are considering certain preferences:

- You will buy the shoes only if they are pink **and** grey
- You will buy the shoes if they are entirely pink **or** entirely grey, **or** if they are pink and grey
- You will buy the shoes if they are grey, but **not** if they have any pink

### The power of multiple conditions

For data analysts, the real power of Boolean logic comes from being able to combine multiple conditions in a single statement. For example, if you wanted to filter for shoes that were grey or pink, and waterproof, you could construct a Boolean statement such as `IF ((Color = 'Grey') OR (Color = 'Pink')) AND (Waterproof = 'True')`. Notice that you can use parentheses to group your conditions together.

Whether you are doing a search for new shoes or applying this logic to your database queries, Boolean logic lets you create multiple conditions to filter your results.

## Transforming data

Data transformation is the process of changing the data's format, structure, or values. As a data analyst, there is a good chance you will need to transform data at some point to make it easier for you to analyze it.

Data transformation usually involves:

- Adding, copying, or replicating data
- Deleting fields or records
- Standardizing the names of variables
- Renaming, moving, or combining columns in a database
- Joining one set of data with another
- Saving a file in a different format. For example, saving a spreadsheet as a comma separated values (CSV) file

Goals for data transformation might be:

- Data organization: better organized data is easier to use
- Data compatibility: different applications or systems can then use the same data
- Data migration: data with matching formats can be moved from one system to another
- Data merging: data with the same organization can be merged together
- Data enhancement: data can be displayed with more detailed fields
- Data comparison: apples-to-apples comparisons of the data can then be made

Shape of data:

- **Long data** is data where **each row contains a single data point** for a particular item.
- **Wide data** is data where **each row contains multiple data points** for the particular items identified in the columns.

![Example of long data](https://github.com/x-square/visual-resources/blob/main/data-long.png?raw=true 'Example of long data')

![Example of wide data](https://github.com/x-square/visual-resources/blob/main/data-wide.png?raw=true 'Example of wide data')

You might notice that all the data included in the long format is also in the wide format. But wide data is easier to read and understand. That is why data analysts typically transform long data to wide data more often than they transform wide data to long data.

The following table summarizes when each format is preferred:

- Wide data is preferred when
    - Creating tables and charts with a few variables about each subject
    - Comparing straightforward line graphs
- Long data is preferred when
    - Storing a lot of variables about each subject. For example, 60 years worth of interest rates for each bank
    - Performing advanced statistical analysis or graphing

## Data anonymization

**Personally identifiable information** (PII), is information that can be used by itself or with other data to track down a person's identity. Imagine a world where we all had access to each other's addresses, account numbers, and other identifiable information. That would invade a lot of people's privacy and make the world less safe. Data anonymization is one of the ways we can keep data private and secure!

Healthcare and financial data are two of the most sensitive types of data. These industries rely a lot on data anonymization techniques. After all, the stakes are very high. That's why data in these two industries usually goes through **de-identification**, which is **a process used to wipe data clean of all personally identifying information**.

Data anonymization is used in just about every industry. That is why it is so important for data analysts to understand the basics. Here is a list of data that is often anonymized:

- Telephone numbers
- Names
- License plates and license numbers
- Social security numbers
- IP addresses
- Medical records
- Email addresses
- Photographs
- Account numbers

## The open data debate

In data analytics, open data is part of data ethics, which has to do with using data ethically. Openness refers to free access, usage, and sharing of data. But for data to be considered open, it has to:

- Be available and accessible to the public as a complete dataset
- Be provided under terms that allow it to be reused and redistributed
- Allow universal participation so that anyone can use, reuse, and redistribute the data

Data can only be considered open when it meets all three of these standards.

### What data should be publicly available?

Open data's major advantage lies in its widespread usability. Credible databases become more accessible, fostering scientific collaboration, research progress, analytical capabilities, and informed decision-making. However, it's crucial to consider the impact on individuals represented in public, open data.

**Third-party data**, collected by entities without a direct user relationship, involves gathering information, as discussed earlier. For instance, these entities might compile data on website visitors to create audience profiles, enhancing understanding of user behavior and enabling more targeted advertising.

**Personal identifiable information** is data likely to identify and disclose information about an individual. Safeguarding such data is crucial. PII encompasses details like addresses, credit card information, social security numbers, medical records, and more.

Everyone wants to keep personal information about themselves private. Because third-party data is readily available, it is important to balance the openness of data with the privacy of individuals.

### Sites and resources for open data

Luckily for data analysts, there are lots of trustworthy sites and resources available for open data. It is important to remember that even reputable data needs to be constantly evaluated, but these websites are a useful starting point:

- [US government data site](https://www.data.gov): Data.gov is one of the most comprehensive data sources in the US. This resource gives users the data and tools that they need to do research, and even helps them develop web and mobile applications and design data visualizations.
- [US Census Bureau](https://www.census.gov/data.html): This open data source offers demographic information from federal, state, and local governments, and commercial entities in the US too.
- [Open Data Network](https://www.opendatanetwork.com): This data source has a really powerful search engine and advanced filters. Here, you can find data on topics like finance, public safety, infrastructure, and housing and development.
- [Google Cloud Public Datasets](https://cloud.google.com/public-datasets): There are a selection of public datasets available through the Google Cloud Public Dataset Program that you can find already loaded into BigQuery.
- [Dataset Search](https://datasetsearch.research.google.com): The Dataset Search is a search engine designed specifically for data sets; you can use this to search for specific data sets.
- [BigQuery](https://cloud.google.com/bigquery/public-data): this hosts 150+ public datasets you can access and use.
- [Global Health Observatory data](https://www.who.int/data/collections): You can search for datasets from this page or explore featured data collections from the World Health Organization.
- [The Cancer Imaging Archive dataset](https://cloud.google.com/healthcare-api/docs/resources/public-datasets/idc): Just like the earlier dataset, this data is hosted by the Google Cloud Public Datasets and can be uploaded to BigQuery.
- [Naitonal Climatic Data Center](https://www.ncei.noaa.gov/weather-climate-links): The NCDC Quick Links page has a selection of datasets you can explore. 
- [NOAA Public Dataset Gallery](https://www.climate.gov/maps-data/all?listingMain=datasetgallery): The NOAA Public Dataset Gallery contains a searchable collection of public datasets.
- [UNICEF State of the World's Children](https://data.unicef.org/resources/dataset/sowc-2019-statistical-tables): This dataset from UNICEF includes a collection of tables that can be downloaded.
- [CPS Labor Force Statistics](https://www.bls.gov/cps/tables.htm): This page contains links to several available datasets that you can explore.
- [The Stanford Open Policing Project](https://openpolicing.stanford.edu): This dataset can be downloaded as a .CSV file for your own use.

## Databases in data analytics

Databases enable analysts to manipulate, store, and process data. This helps them search through data a lot more efficiently to get the best insights.

### Relational databases

A **relational** database is a database that contains a series of tables that can be connected to show relationships. Basically, they allow data analysts to organize and link data based on what the data has in common.

In a **non-relational** table, you will find all of the possible variables you might be interested in analyzing all grouped together. This can make it really hard to sort through. This is one reason why relational databases are so common in data analysis. They simplify a lot of analysis processes and make data easier to find and use across an entire database.

### Key to relational databases

Tables in a relational database are connected by the fields they have in common. You might remember learning about primary and foreign keys before. As a quick refresher, a **primary key** is an identifier that references a column in which each value is unique. In other words, it's a column of a table that is used to uniquely identify each record within that table. The value assigned to the primary key in a particular row must be unique within the entire table. For example, if customer_id is the primary key for the customer table, no two customers will ever have the same customer_id.

By contrast, a **foreign key** is a field within a table that is a primary key in another table. A table can have only one primary key, but it can have multiple foreign keys. These keys are what create the relationships between tables in a relational database, which helps organize and connect data across multiple tables in the database.

Some tables don't require a primary key. For example, a revenue table can have multiple foreign keys and not have a primary key. A primary key may also be constructed using multiple columns of a table. This type of primary key is called a composite key. For example, if customer_id and location_id are two columns of a **composite key** for a customer table, the values assigned to those fields in any given row must be unique within the entire table.

![Example of database keys](https://github.com/x-square/visual-resources/blob/main/database-keys.png?raw=true 'Example of database keys')

## Inspecting a dataset: A guided, hands-on tour

As a data analyst, you'll use data to answer questions and solve problems. When you analyze data and draw conclusions, you are generating insights that can influence business decisions, drive positive change, and help your stakeholders meet their goals.

Before you begin an analysis, it's important to inspect your data to determine if it contains the specific information you need to answer your stakeholders' questions. In any given dataset, it may be the case that:

- The data is not there (you have sandwich data, but you need pizza data)
- The data is insufficient (you have pizza data for June 1-7, but you need data for the entire month of June)
- The data is incorrect (your pizza data lists the cost of a slice as \$250, which makes you question the validity of the dataset)

Inspecting your dataset will help you pinpoint what questions are answerable and what data is still missing. You may be able to recover this data from an external source or at least recommend to your stakeholders that another data source be used.

### Scenario

You are a data analyst working for an ice cream company. Management is interested in improving the company's ice cream sales.

The company has been collecting data about its sales but not a lot. The available data is from an internal data source and is based on sales for 2019. You've been asked to review the data and provide some insight into the company's ice cream sales. Ideally, management would like answers to the following questions:

- What is the most popular flavor of ice cream?
- How does temperature affect sales?
- How do weekends and holidays affect sales?
- How does profitability differ for new versus returning customers?

### Inspect the data

#### Question 1: What is the most popular flavor of ice cream?

To discover the most popular flavor, you first need to define what is meant by **popular**. Is the most popular flavor the one that generated the most revenue in 2019? Or is it the flavor that had the largest number of units sold in 2019? Sometimes your measurement choices are limited by what data you have. You can review your spreadsheet to find out if either of these definitions of **popular** make sense based on the available data.

In this case, you can discover what the most popular flavor is by using units sold as your measure. In particular, you can use the units sold column to calculate the total number of units sold during the year for each flavor. Unfortunately, the dataset does not provide the annual sales amount by flavor. In this case, your next step would be to ask your stakeholders if the annual sales per flavor data is available from another source. If not, you can add a statement about the current data's limitations to your analysis.

![Example of sales data by ice cream flavour](https://github.com/x-square/visual-resources/blob/main/data-ice-cream-flavour.png?raw=true 'Example of sales data by ice cream flavour')

#### Question 2: How does temperature affect sales?

The column headers are temperature and sales. The data may show total 2019 sales per temperature (for instance, the first entry might sum up \$36.69 in sales for three separate days that each had a high of 60 degrees). Or, the data may show a snapshot of sales and temperature for each day in 2019 (for instance, the first entry might refer to a single day with a high of 60 degrees and \$39.69 in sales).

So, which is it? It's probably a daily snapshot because there are 365 entries for temperature, and multiple rows with the same temperature and different sales values. This implies that each entry is for a single day and not a summary of multiple days. However, without more information, you can't be certain. Plus, you don't know if the current data is listed in consecutive order by date or in a different order. Your next step would be to contact the owner of the dataset for clarification.

If it turns out that temperature does affect sales, you'll be able to offer your stakeholders an insight such as the following: **When daily highs are above X degrees, average ice cream sales increase by Y amount. So the business should plan on increasing inventory during these times to maximize sales**.

![Example of sales data by temperature](https://github.com/x-square/visual-resources/blob/main/data-ice-cream-temperature.png?raw=true 'Example of sales data by temperature')

#### Question 3: How do weekends and holidays affect sales?

You can use this data to determine whether a specific date falls on a weekend or holiday and add a column to your sheet that reflects this information. Then, you can find out whether sales on the weekends and holidays are greater than sales on other days. This will be useful to know for inventory planning and marketing purposes.

![Example of sales data by weekend and holiday](https://github.com/x-square/visual-resources/blob/main/data-ice-cream-weekend.png?raw=true 'Example of sales data by weekend and holida')

#### Question 4: How does profitability differ for new customers versus returning customers?

Your dataset does not contain sales data related to new customers. Without this data, you won't be able to answer your final question. However, it may be the case that the company collects customer data and stores it in a different data table.

If so, your next step would be to find out how to access the company's customer data. You can then join the revenue sales data to the customer data table to categorize each sale as from a new or returning customer and analyze the difference in profitability between the two sets of customers. This information will help your stakeholders develop marketing campaigns for specific types of customers to increase brand loyalty and overall profitability.

### Conclusion

When working on analytics projects, you won't always have all the necessary or relevant data at your disposal. In many of these cases, you can turn to other data sources to fill in the gaps.

Despite the limitations of your dataset, it's still possible to offer your stakeholders some valuable insights. For next steps, your best plan of action will be to take the initiative to ask questions, identify other relevant datasets, or do some research on your own. No matter what data you're working with, carefully inspecting your data makes a big impact on the overall quality of your analysis.

## Metadata is as important as the data itself

To put it simply, metadata is data about data. In database management, it provides information about other data and helps data analysts interpret the contents of the data within a database.

Regardless of whether you are working with a large or small quantity of data, metadata is the mark of a knowledgeable analytics team, helping to communicate about data across the business and making it easier to reuse data. In essence, metadata tells the who, what, when, where, which, how, and why of data.

### Elements of data

- Title and description
    - What is the name of the file or website you are examining? What type of content does it contain?
- Tags and categories
    - What is the general overview of the data that you have? Is the data indexed or described in a specific way?
- Who created it and when
    - Where did the data come from, and when was it created? Is it recent, or has it existed for a long time?
- Who last modified it and when
    - Were any changes made to the data? If yes, were the modifications recent?
- Who can access or update it
    - Is this dataset public? Are special permissions needed to customize or modify the dataset?

### Examples of metadata

In today's digital world, metadata is everywhere, and it is becoming a more common practice to provide metadata on a lot of media and information you interact with. Here are some real-world examples of where to find metadata:

- Photos
    - Whenever a photo is captured with a camera, metadata such as camera filename, date, time, and geolocation are gathered and saved with it.
- Emails
    - When an email is sent or received, there is lots of visible metadata such as subject line, the sender, the recipient and date and time sent. There is also hidden metadata that includes server names, IP addresses, HTML format, and software details.
- Spreadsheets and documents
    - Spreadsheets and documents are already filled with a considerable amount of data so it is no surprise that metadata would also accompany them. Titles, author, creation date, number of pages, user comments as well as names of tabs, tables, and columns are all metadata that one can find in spreadsheets and documents.
- Websites
    - Every web page has a number of standard metadata fields, such as tags and categories, site creator's name, web page title and description, time of creation and any iconography.
- Digital files
    - Usually, if you right click on any computer file, you will see its metadata. This could consist of file name, file size, date of creation and modification, and type of file.
- Books
    - Metadata is not only digital. Every book has a number of standard metadata on the covers and inside that will inform you of its title, author's name, a table of contents, publisher information, copyright description, index, and a brief description of the book's contents.

### Data as you know it

Knowing the content and context of your data, as well as how it is structured, is very valuable in your career as a data analyst. When analyzing data, it is important to always understand the full picture. It is not just about the data you are viewing, but how that data comes together. Metadata ensures that you are able to find, use, preserve, and reuse data in the future. Remember, it will be your responsibility to manage and make use of data in its entirety; metadata is as important as the data itself.

## File structure and naming convention

| **Formatting convention** | **Example** |
|---------------------------|-------------|
| Format dates as yyyymmdd | SalesReport20201125|
| Lead revision numbers with 0 | SalesReport20201125v02 |
| Use hyphens, underscores, or capitalized letters | <li> sales-report-2020-11-25-v02 <li> SalesReport_2020_11_25_v02 |

: Best practices for filename conventions to follow

### Best practices for file naming conventions

Review the following file naming recommendations:

- Work out and agree on file naming conventions early on in a project to avoid renaming files again and again.
- Align your file naming with your team's or company's existing file-naming conventions.
- Ensure that your file names are meaningful; consider including information like project name and anything else that will help you quickly identify (and use) the file for the right purpose.
- Include the date and version number in file names; common formats are YYYYMMDD for dates and v## for versions (or revisions).
- Create a text file as a sample file with content that describes (breaks down) the file naming convention and a file name that applies it.
- Avoid spaces and special characters in file names. Instead, use dashes, underscores, or capital letters. Spaces and special characters can cause errors in some applications.

### Best practices for keeping files organized

Remember these tips for staying organized as you work with files:

- Create folders and subfolders in a logical hierarchy so related files are stored together.
- Separate ongoing from completed work so your current project files are easier to find. Archive older files in a separate folder, or in an external storage location.
- If your files aren't automatically backed up, manually back them up often to avoid losing important work.

## The battle between security and data analytics

Data security means protecting data from unauthorized access or corruption by putting safety measures in place. Usually the purpose of data security is to keep unauthorized users from accessing or viewing sensitive data. Data analysts have to find a way to balance data security with their actual analysis needs. This can be tricky. We want to keep our data safe and secure, but we also want to use it as soon as possible so that we can make meaningful and timely observations.

Examples of security measures:

- **Encryption** uses a unique algorithm to alter data and make it unusable by users and applications that don't know the algorithm. This algorithm is saved as a **key** which can be used to reverse the encryption; so if you have the key, you can still use the data in its original form.
- **Tokenization** replaces the data elements you want to protect with randomly generated data referred to as a **token**. The original data is stored in a separate location and mapped to the tokens. To access the complete original data, the user or application needs to have permission to use the tokenized data and the token mapping. This means that even if the tokenized data is hacked, the original data is still safe and secure in a separate location.

# Process data from dirty to clean

## Data integrity and compliance

Think about what would happen if you were working as a data analyst for a global company and didn't check date formats. Well, your data integrity would probably be questionable. Any analysis of the data e.g. 12/10/20 would be inaccurate. Imagine ordering extra inventory for December when it was actually needed in October!

A good analysis depends on the integrity of the data, and data integrity usually depends on using a common format. So it is important to double-check how dates are formatted to make sure what you think is December 10, 2020 isn't really October 12, 2020, and vice versa.

Here are some other things to watch out for:

- Data replication compromising data integrity
    - Imagine you ask your international counterparts to verify dates and stick to one format. One analyst copies a large dataset to check the dates. But because of memory issues, only part of the dataset is actually copied. The analyst would be verifying and standardizing incomplete data. That partial dataset would be certified as compliant but the full dataset would still contain dates that weren't verified. Two versions of a dataset can introduce inconsistent results. A final audit of results would be essential to reveal what happened and correct all dates.
- Data transfer compromising data integrity
    - Another analyst checks the dates in a spreadsheet and chooses to import the validated and standardized data back to the database. But suppose the date field from the spreadsheet was incorrectly classified as a text field during the data import (transfer) process. Now some of the dates in the database are stored as text strings. At this point, the data needs to be cleaned to restore its integrity. 
- Data manipulation compromising data integrity
    - When checking dates, another analyst notices what appears to be a duplicate record in the database and removes it. But it turns out that the analyst removed a unique record for a company's subsidiary and not a duplicate record for the company. Your dataset is now missing data and the data must be restored for completeness.

As you progress in your data journey, you'll come across many types of data constraints (or criteria that determine validity). The table below offers definitions and examples of data constraint terms you might come across.

| **Data constraint** | **Definition** | **Examples** |
|---------------------|----------------|--------------|
| Data type | Values must be of a certain type: date, number, percentage, Boolean | If the data type is a date, a single number like 30 would fail the constraint and be invalid |
| Data range | Values must fall between predefined maximum and minimum values | If the data range is 10-20, a value of 30 would fail the constraint and be invalid |
| Mandatory | Values can't be left blank or empty | If age is mandatory, that value must be filled in |
| Unique | Values can't have a duplicate | Two people can't have the same mobile phone number within the same service area |
| Regular expression patterns | Values must match a prescribed pattern | A phone number must match ###-###-#### (no other characters allowed) |
| Cross-field validation | Certain conditions for multiple fields must be satisfied | Values are percentages and values from multiple fields must add up to 100% |
| Primary key | (Databases only) value must be unique per column | A database table can't have two rows with the same primary key value. A primary key is an identifier in a database that references a column in which each value is unique. More information about primary and foreign keys is provided later in the program. |
| Set-membership | (Databases only) values for a column must come from a set of discrete values | Value for a column must be set to Yes, No, or Not Applicable |
| Foreign key | (Databases only) values for a column must be unique values coming from a column in another table | In a US taxpayer database, the State column must be a valid state or territory with the set of acceptable values defined in a separate States table |
| Accuracy | The degree to which the data conforms to the actual entity being measured or described | If values for zip codes are validated by street location, the accuracy of the data goes up |
| Completeness | The degree to which the data contains all desired components or measures | If data for personal profiles required hair and eye color, and both are collected, the data is complete |
| Consistency | The degree to which the data is repeatable from different points of entry or collection | If a customer has the same address in the sales and repair databases, the data is consistent |

: Data constraints and examples

## Well-aligned objectives and data

You can gain powerful insights and make accurate conclusions when data is well-aligned to business objectives. As a data analyst, alignment is something you will need to judge. Good alignment means that the data is relevant and can help you solve a business problem or determine a course of action to achieve a given business objective.

### Business case A

#### Clean data + alignment to business objective = accurate conclusions

Account managers at Impress Me, an online content subscription service, want to know how soon users view content after their subscriptions are activated. 

To start off, the data analyst verifies that the data exported to spreadsheets is clean and confirms that the data needed (when users access content) is available. Knowing this, the analyst decides there is good alignment of the data to the business objective. All that is missing is figuring out exactly how long it takes each user to view content after their subscription has been activated.

![Example of relevant data in spreadsheet](https://github.com/x-square/visual-resources/blob/main/data-spreadsheet.png?raw=true 'Example of relevant data in spreadsheet')

### Business case B

#### Alignment to business objective + additional data cleaning = accurate conclusions 

Cloud Gate, a software company, recently hosted a series of public webinars as free product introductions. The data analyst and webinar program manager want to identify companies that had five or more people attend these sessions. They want to give this list of companies to sales managers who can follow up for potential sales.

| **Name** | **Research methods** | **Additional information** |
|----------|----------------------|----------------------------|
| Email Address | `xxxxx@company.com`  | Required information attendees had to submit |
| Company | \<company name\> | Optional information attendees could provide |

: Webinar attendance data includes the fields

The webinar attendance data seems to align with the business objective. But the data analyst and program manager decide that some **data cleaning** is needed before the analysis. They think data cleaning is required because:

- The company name wasn't a mandatory field. If the company name is blank, it might be found from the email address. For example, if the email address is `username@google.com`, the company field could be filled in with Google for the data analysis. This data cleaning step assumes that people with company-assigned email addresses attended a webinar for business purposes.
- Attendees could enter any name. Since attendance across a series of webinars is being looked at, they need to validate names against unique email addresses. For example, if Joe Cox attended two webinars but signed in as Joe Cox for one and Joseph Cox for the other, he would be counted as two different people. To prevent this, they need to check his unique email address to determine that he was the same person. After the validation, Joseph Cox could be changed to Joe Cox to match the other instance.

### Business case C

#### Alignment to business objective + newly discovered variables + constraints = accurate conclusions

An after-school tutoring company, A+ Education, wants to know if there is a minimum number of tutoring hours needed before students have at least a 10% improvement in their assessment scores.

The data analyst thinks there is good alignment between the data available and the business objective because:

- Students log in and out of a system for each tutoring session, and the number of hours is tracked
- Assessment scores are regularly recorded

After looking at the data, the data analyst discovers that there are **other variables** to consider. Some students had consistent weekly sessions while other students had scheduled sessions more randomly even though their total number of tutoring hours was the same. The data doesn't align as well with the original business objective as first thought, so the analyst adds a **data constraint** to focus only on the students with consistent weekly sessions. This modification helps to get a more accurate picture about the enrolment time needed to achieve a 10% improvement in assessment scores.

## What to do when you find an issue with your data

When you are getting ready for data analysis, you might realize you don't have the data you need or you don't have enough of it. In some cases, you can use what is known as proxy data in place of the real data. Think of it like substituting oil for butter in a recipe when you don't have butter. In other cases, there is no reasonable substitute and your only option is to collect more data.

Consider the following data issues and suggestions on how to work around them:

### No data

| **Possible Solutions** | **Examples of solutions in real life** |
|------------------------|----------------------------------------|
| Gather the data on a small scale to perform a preliminary analysis and then request additional time to complete the analysis after you have collected more data | If you are surveying employees about what they think about a new performance and bonus plan, use a sample for a preliminary analysis. Then, ask for another 3 weeks to collect the data from all employees. |
| If there isn't time to collect data, perform the analysis using proxy data from other datasets. This is the most common workaround. | If you are analyzing peak travel times for commuters but don't have the data for a particular city, use the data from another city with a similar size and demographic. |

: Data issue of no data

### Too little data

| **Possible Solutions** | **Examples of solutions in real life** |
|------------------------|----------------------------------------|
| Do the analysis using proxy data along with actual data. | If you are analyzing trends for owners of golden retrievers, make your dataset larger by including the data from owners of labradors. |
| Adjust your analysis to align with the data you already have. | If you are missing data for 18 to 24-year-olds, do the analysis but note the following limitation in your report: this conclusion applies to adults 25 years and older only. |

: Data issue of too little data

### Wrong data, including data with errors

| **Possible Solutions** | **Examples of solutions in real life** |
|------------------------|----------------------------------------|    
| If you have the wrong data because requirements were misunderstood, communicate the requirements again. | If you need the data for female voters and received the data for male voters, restate your needs. |
| Identify errors in the data and, if possible, correct them at the source by looking for a pattern in the errors. | If your data is in a spreadsheet and there is a conditional statement or boolean causing calculations to be wrong, change the conditional statement instead of just fixing the calculated values. |
| If you can't correct data errors yourself, you can ignore the wrong data and go ahead with the analysis if your sample size is still large enough and ignoring the data won't cause systematic bias. | If your dataset was translated from a different language and some of the translations don't make sense, ignore the data with bad translation and go ahead with the analysis of the other data. |

: Data issue of wrong data and errors

Use the following decision tree as a reminder of how to deal with data errors or not enough data:

![Decision tree of how to deal with data errors or not enough data](https://github.com/x-square/visual-resources/blob/main/data-errors-not-enough.png?raw=true 'Decision tree of how to deal with data errors or not enough data')

## Calculating sample size

| **Terminology** | **Definitions** |
|-----------------|-----------------|
| **Population** | The entire group that you are interested in for your study. For example, if you are surveying people in your company, the population would be all the employees in your company. |
| **Sample** | A subset of your population. Just like a food sample, it is called a sample because it is only a taste. So if your company is too large to survey every individual, you can survey a representative sample of your population. |
| **Margin of error** | Since a sample is used to represent a population, the sample's results are expected to differ from what the result would have been if you had surveyed the entire population. This difference is called the margin of error. The smaller the margin of error, the closer the results of the sample are to what the result would have been if you had surveyed the entire population. |
| **Confidence level** | How confident you are in the survey results. For example, a `95%` confidence level means that if you were to run the same survey 100 times, you would get similar results 95 of those 100 times. Confidence level is targeted before you start your study because it will affect how big your margin of error is at the end of your study. |
| **Confidence interval** | The range of possible values that the population's result would be at the confidence level of the study. This range is the sample result plus and minus the margin of error. Briefly, `confidence interval = sample mean ± margin of error`. |
| **Effect size** | The effect size is a quantitative measure of the magnitude of the experimental effect. The larger the effect size the stronger the relationship between two variables. You can look at the effect size when comparing any two groups e.g. control group and experimental group to see how substantially different they are. A significant *p* value tells us that an intervention works, whereas an effect size tells us how much it works. |
| **Statistical power** | It can be calculated and reported e.g. `0.8` or `80%` for a completed experiment to comment on the confidence one might have in the conclusions drawn from the results of the study. It can also be used as a tool to estimate the number of observations or sample size required in order to detect an effect in an experiment. |

: Statistical terms and definitions

When figuring out a sample size, here are things to keep in mind:

- Don't use a sample size less than 30. It has been statistically proven that 30 is the smallest sample size where an average result of a sample starts to represent the average result of a population.
    - This recommendation is based on the **Central Limit Theorem** in the field of probability and statistics. As sample size increases, the results more closely resemble the normal (bell-shaped) distribution from a large number of samples.
    - A sample of 30 is the smallest sample size for which the Central Limit Theorem is still valid. Researchers who rely on **regression analysis** – statistical methods to determine the relationships between controlled and dependent variables – also prefer a minimum sample of 30.
- The confidence level most commonly used is 95%, but 90% can work in some cases.
- Increase the sample size to meet specific needs of your project
    - For a higher confidence level, use a larger sample size
    - To decrease the margin of error, use a larger sample size
    - For greater statistical significance, use a larger sample size

### Why a minimum sample of 30?

This recommendation is based on the **Central Limit Theorem** in the field of probability and statistics. As sample size increases, the results more closely resemble the normal (bell-shaped) distribution from a large number of samples. A sample of 30 is the smallest sample size for which the CLT is still valid. Researchers who rely on **regression analysis** – statistical methods to determine the relationships between controlled and dependent variables – also prefer a minimum sample of 30.

### Sample sizes vary by business problem

If you live in a city with a population of 200,000 and get 180,000 people to respond to a survey, that is a large sample size. But without actually doing that, what would an acceptable, smaller sample size look like? 

Would 200 be alright if the people surveyed represented every district in the city? It depends on the stakes:

- A sample size of 200 might be large enough if your business problem is to find out how residents felt about the new library
- A sample size of 200 might not be large enough if your business problem is to determine how residents would vote to fund the library

You could probably accept a larger margin of error surveying how residents feel about the new library versus surveying residents about how they would vote to fund it. For that reason, you would most likely use a larger sample size for the voter survey.

## Sample size calculator

In order to use a sample size calculator, you need to have the **population size**, **confidence level**, and the acceptable **margin of error** already decided so you can input them into the tool. If this information is ready to go, check out these sample size calculators below:

- [SurveyMonkey](https://www.surveymonkey.com/mp/sample-size-calculator 'Sample size calculator')
- [Raosoft](http://www.raosoft.com/samplesize.html 'Sample size calculator')

## All about margin of error

Margin of error is the maximum amount that the sample results are expected to differ from those of the actual population. More technically, the margin of error defines a range of values below and above the average result for the sample. The average result for the entire population is expected to be within that range. We can better understand margin of error by using some examples below.

### Margin of error in baseball

Imagine you are playing baseball and that you are up at bat. The crowd is roaring, and you are getting ready to try to hit the ball. The pitcher delivers a fast ball travelling about 90-95mph, which takes about 400 milliseconds (ms) to reach the catcher's glove. You swing and miss the first pitch because your timing was a little off. You wonder if you should have swung slightly earlier or slightly later to hit a home run. That time difference can be considered the margin of error, and it tells us how close or far your timing was from the average home run swing.

### Margin of error in marketing

For example, suppose you are conducting an A/B test to compare the effectiveness of two different email subject lines to entice people to open the email. You find that subject line A: `Special offer just for you` resulted in a 5% open rate compared to subject line B: `Don't miss this opportunity` at 3%.

Does that mean subject line A is better than subject line B? It depends on your margin of error. If the margin of error was 2%, then subject line A's actual open rate or confidence interval is somewhere between 3% and 7%. Since the lower end of the interval overlaps with subject line B's results at 3%, you can't conclude that there is a statistically significant difference between subject line A and B. Examining the margin of error is important when making conclusions based on your test results.

### Calculate your margin of error

All you need is **population size**, **confidence level**, and **sample size**.

- [SurveyMonkey](https://uk.surveymonkey.com/mp/margin-of-error-calculator 'Margin of error calculator')
- [CheckMarket](https://www.checkmarket.com/sample-size-calculator/#sample-size-margin-of-error-calculator 'Margin of error calculator')

## What is dirty data?

![Types of dirty data](https://github.com/x-square/visual-resources/blob/main/data-dirty.png?raw=true 'Types of dirty data')

| **Description** | **Possible causes** | **Potential harm to businesses** |
|-----------------|---------------------|----------------------------------|
| Duplicate data that shows up more than once | Manual data entry, batch data imports, or data migration | Skewed metrics or analyses, inflated or inaccurate counts or predictions, or confusion during data retrieval |
| Outdated data that should be replaced with newer and more accurate information | People changing roles or companies, or software and systems becoming obsolete | Inaccurate insights, decision-making, and analytics |
| Incomplete data that is missing important fields | Improper data collection or incorrect data entry | Decreased productivity, inaccurate insights, or inability to complete essential services |
| Inaccurate data that is complete but inaccurate | Human error inserted during data input, fake information, or mock data | Inaccurate insights or decision-making based on bad information resulting in revenue loss |
| Inconsistent data that uses different formats to represent the same thing | Data stored incorrectly or errors inserted during data transfer | Contradictory data points leading to confusion or inability to classify or segment customers |

: Types of dirty data
 
### Business impact of dirty data

Here are a few impacts cited for certain industries from a previous search:

- [Banking](https://sloanreview.mit.edu/article/seizing-opportunity-in-data-quality "Seizing opportunity in data quality"): Inaccuracies cost companies between 15% and 25% of revenue
- [Digital commerce](https://www.demandgen.com/dirty-data-what-is-it-costing-you "Dirty data: What is it costing you?"): Up to 25% of B2B database contacts contain inaccuracies
- [Marketing and sales](https://www.dqglobal.com/blog/why-bad-data-is-wasting-your-marketing-efforts "Why bad data is a waste of your marketing efforts"): 99% of companies are actively tackling data quality in some way
- [Healthcare](https://www.techtarget.com/searchdatamanagement/tip/How-data-duplication-in-healthcare-is-diagnosed 'How data duplication in healthcare is diagnosed'): Duplicate records can be 10% and even up to 20% of a hospital's electronic health records

## Common data-cleaning pitfalls

![Errors you might come across while cleaning your data](https://github.com/x-square/images/blob/main/data-cleaning-errors.png?raw=true 'Errors you might come across while cleaning your data')

Top ten lists for data cleaning:

- [Microsoft Excel](https://support.microsoft.com/en-us/office/top-ten-ways-to-clean-your-data-2844b620-677c-47a7-ac3e-c2e157d1db19 'Top ten ways to clean your data')
- [Google Sheets](https://support.google.com/a/users/answer/9604139?hl=en#zippy= "Tips to format and clean up data")

## Data-cleaning verification checklist

### Correct the most common problems

- **Sources of errors**: Did you use the right tools and functions to find the source of the errors in your dataset?
- **Null data**: Did you search for NULLs using conditional formatting and filters?
- **Misspelled words**: Did you locate all misspellings?
- **Mistyped numbers**: Did you double-check that your numeric data has been entered correctly?
- **Extra spaces and characters**: Did you remove any extra spaces or characters using the **TRIM** function?
- **Duplicates**: Did you remove duplicates in spreadsheets using the **Remove Duplicates** function or **DISTINCT** in SQL?
- **Mismatched data types**: Did you check that numeric, date, and string data are typecast correctly?
- **Messy (inconsistent) strings**: Did you make sure that all of your strings are consistent and meaningful?
- **Messy (inconsistent) date formats**: Did you format the dates consistently throughout your dataset?
- **Misleading variable labels (columns)**: Did you name your columns meaningfully?
- **Truncated data**: Did you check for truncated or missing data that needs correction?
- **Business logic**: Did you check that the data makes sense given your knowledge of the business?

### Review the goal of your project after data cleaning

- Confirm the business problem 
- Confirm the goal of the project
- Verify that data can solve the problem and is aligned to the goal 

## Workflow automation

| **Task** | **Can it be automated?** | **Why?** |
|----------|--------------------------|----------|
| Communicating with your team and stakeholders | No | Communication is key to understanding the needs of your team and stakeholders as you complete the tasks you are working on. There is no replacement for person-to-person communications. |
| Presenting your findings | No | Presenting your data is a big part of your job as a data analyst. Making data accessible and understandable to stakeholders and creating data visualizations can't be automated for the same reasons that communications can't be automated. |
| Preparing and cleaning data | Partially | Some tasks in data preparation and cleaning can be automated by setting up specific processes, like using a programming script to automatically detect missing values. |
| Data exploration | Partially | Sometimes the best way to understand data is to see it. Luckily, there are plenty of tools available that can help automate the process of visualising data. These tools can speed up the process of visualizing and understanding the data, but the exploration itself still needs to be done by a data analyst. |
| Modelling the data | Yes | Data modelling is a difficult process that involves lots of different factors Luckily there are tools that can completely automate the different stages. |

: What can be automated?

## Embrace changelogs

Engineers use **engineering change orders** to keep track of new product design details and proposed changes to existing products. Writers use document revision histories to keep track of changes to document flow and edits. And data analysts use changelogs to keep track of data transformation and cleaning.

![Example of changelogs](https://github.com/x-square/visual-resources/blob/main/changelogs.png?raw=true 'Example of changelogs')

Typically, a changelog records this type of information:  

- Data, file, formula, query, or any other component that changed
- Description of what changed
- Date of the change
- Person who made the change
- Person who approved the change 
- Version number 
- Reason for the change

Here is how a version control system affects a change to a query:

- A company has official versions of important queries in their **version control system**.
- An analyst makes sure the most up-to-date version of the query is the one they will change. This is called **syncing**.
- The analyst makes a change to the query.
- The analyst might ask someone to review this change. This is called a **code review** and can be informally or formally done. An informal review could be as simple as asking a senior analyst to take a look at the change.
- After a reviewer approves the change, the analyst submits the updated version of the query to a repository in the company's version control system. This is called a **code commit**. A best practice is to document exactly what the change was and why it was made in a comments area. Going back to our example of a query that pulls daily revenue, a comment might be `updated revenue to include revenue coming from the new product, Calypso`.
- After the change is **submitted**, everyone else in the company will be able to access and use this new query when they sync to the most up-to-date queries stored in the version control system.
- If the query has a problem or business needs change, the analyst can **undo** the change to the query using the version control system. The analyst can look at a chronological list of all changes made to the query and who made each change. Then, after finding their own change, the analyst can **revert** to the previous version.
- The query is back to what it was before the analyst made the change. And everyone at the company sees this reverted, original query, too.

## PAR method versus STAR method

**By using PAR, we can showcase our skills and impact in a brief and measurable manner.**    

> [!TIP]
> **PAR method**
>
> - Describe the **problem** you faced
> - Explain the **action** you took to address the problem
> - Share the **result** you achieved through your actions

- Counterexample: ~~Was responsible for writing two blogs a month~~
- Example 1: Earned little known website over 2,000 organic clicks through strategic blogging
    - Problem: little known website
    - Action: through strategic blogging 
    - Result: earn over 2,000 organic clicks
- Example 2: Effectively implemented and communicated daily workflow procedures to fellow team members, resulting in **a 15% increase** in productivity
    - Problem: previously absent workflow procedures
    - Action: implemented and communicated daily workflow procedures 
    - Result: 15% increase in productivity

STAR method can be confusing as it may ask for repetitive information in both situation and task and steps.

> [!CAUTION]
> STAR method (obsolete)
>
> - Situation you had to deal with to set the context for your story
> - Task you were given to do to achieve the target from the situation
> - Action you took and why was it but not the alternatives
> - Result of your action and what did you learn from the experience

## Advanced functions for speedy data cleaning

![Speed up the data cleaning process](https://github.com/x-square/visual-resources/blob/main/data-cleaning-speed.png?raw=true 'Speed up the data cleaning process')

### Adding professional skills to your resume

As a data analyst, you are often asked to collect and analyze data with a specific purpose in mind. Knowing which platform and language to use helps you analyze the data to decipher which information is important, to probe for any anomalies, prepare questions, assess risks, and so much more.

Common professional skills for entry-level data analysts:

- Structured Query Language
- Spreadsheets
- Data visualization
- Python

### Adding soft skills to your resume

- Analyze your previous work experience and find opportunities to insert a soft skill. For example, if you worked in a restaurant, you could emphasize your communication and adaptability skills that you utilized to effectively function during peak hours.
- Call attention to your problem-solving, presentation, research, and communication skills in previous projects or relevant coursework.
- Add a mix of soft and professional skills in the skills or summary section of your resume.

![Common soft skills you will find in an entry-level data analyst resume](https://github.com/x-square/visual-resources/blob/main/data-analyst-soft-skills.png?raw=true 'Common soft skills you will find in an entry-level data analyst resume')

# Analyze data to answer questions

## Keeping data organized with sorting and filters

You have learned about four phases of analysis: 

- Organize data
- Format and adjust data
- Get input from others
- Transform data 

The organization of datasets is really important for data analysts. Most of the datasets you will use will be organized as tables. Tables are helpful because they let you manipulate your data and categorize it. Having distinct categories and classifications lets you focus on, and differentiate between, your data quickly and easily.

Data analysts also need to format and adjust data when performing an analysis. **Sorting** and **filtering** are two ways you can keep things organized when you format and adjust data to work with it. For example, a filter can help you find errors or outliers so you can fix or flag them before your analysis. **Outliers** are data points that are very different from similarly collected data and might not be reliable values. The benefit of filtering the data is that after you fix errors or identify outliers, you can remove the filter and return the data to its original organization.

Sorting is when you arrange data into a meaningful order to make it easier to understand, analyze, and visualize. It ranks your data based on a specific metric you choose. You can sort data in spreadsheets, SQL databases (when your dataset is too large for spreadsheets), and tables in documents.

Filtering is used when you are only interested in seeing data that meets a specific criteria, and hiding the rest. Filtering is really useful when you have lots of data. You can save time by zeroing in on the data that is really important or the data that has bugs or errors. Most spreadsheets and SQL databases allow you to filter your data in a variety of ways. Filtering gives you the ability to find what you are looking for without too much effort.

## Converting data in spreadsheets

As a data analyst, there are lots of scenarios when you might need to convert data in a spreadsheet:

- [String to date](https://www.ablebits.com/office-addins-blog/excel-convert-text-date/#:~:text=Excel%20DATEVALUE%20function%20%2D%20change%20text,Excel%20recognizes%20as%20a%20date.&text=So%2C%20the%20formula%20to%20convert,stored%20as%20a%20text%20string.)
- [String to numbers](https://www.ablebits.com/office-addins-blog/excel-convert-text-to-number)
- [Combining columns](https://support.microsoft.com/en-us/office/combine-text-from-two-or-more-cells-into-one-cell-81ba0946-ce78-42ed-b3c3-21340eb164a6)
- [Number to percentage](https://support.microsoft.com/en-us/office/format-numbers-as-percentages-de49167b-d603-4450-bcaa-31fba6c7b6b4)

Keep in mind that you may have lots of columns of data that require different formats. Consistency is key, and best practice is to make sure an entire column has the same format.

## Advanced spreadsheet tips and tricks

Google Sheets

- [Keyboard shortcuts for Google Sheets](https://support.google.com/docs/answer/181110 'Keyboard shortcuts for Google Sheets')
- [Google Sheets function list](https://support.google.com/docs/table/25273?hl=en 'Google Sheets function list')
- [23 must-know Google Sheets formulas](https://blog.golayer.io/google-sheets/google-sheets-formulas '23 must-know Google Sheets formulas')
- [18 Google Sheets formulas tips and techniques](https://www.benlcollins.com/spreadsheets/google-sheets-formulas-techniques '18 Google Sheets formulas tips and techniques')

Excel

- [Keyboard shortcuts in Excel](https://support.microsoft.com/en-us/office/keyboard-shortcuts-in-excel-1798d9d5-842a-42b8-9c99-9b7213f0040f?ui=en-US&rs=en-US&ad=US 'Keyboard shortcuts in Excel')
- [222 Excel shortcuts for Windows and Mac](https://exceljet.net/shortcuts '222 Excel shortcuts for Windows and Mac')
- [350 Excel Functions](https://exceljet.net/functions '350 Excel Functions')
- [500 Excel Formulas](https://exceljet.net/formulas '500 Excel Formulas')

### VLOOKUP core concepts

Two common reasons to use VLOOKUP are:

- Populating data in a spreadsheet
- Merging data from one spreadsheet with data in another

## Types of data validation

As a junior data analyst, you might not perform all of these validations. But you could ask if and how the data was validated before you begin working with a dataset. Data validation helps to ensure the integrity of data. It also gives you confidence that the data you are using is clean.

- Data type
    - **Purpose**: Check that the data matches the data type defined for a field.
    - **Example**: Data values for school grades 1-12 must be a numeric data type.
    - **Limitations**: The data value 13 would pass the data type validation but would be an unacceptable value. For this case, data range validation is also needed.
- Data range
    - **Purpose**: Check that the data falls within an acceptable range of values defined for the field.
    - **Example**: Data values for school grades should be values between 1 and 12.
    - **Limitations**: The data value 11.5 would be in the data range and would also pass as a numeric data type. But, it would be unacceptable because there aren't half grades. For this case, data constraint validation is also needed.
- Data constraints
    - **Purpose**: Check that the data meets certain conditions or criteria for a field. This includes the type of data entered as well as other attributes of the field, such as number of characters.
    - **Example**: Data values for school grades 1-12 must be whole numbers.
    - **Limitations**: The data value 13 is a whole number and would pass the content constraint validation. But, it would be unacceptable since 13 isn't a recognized school grade. For this case, data range validation is also needed.
- Data consistency
    - **Purpose**: Check that the data makes sense in the context of other related data.
    - **Example**: Data values for product shipping dates can't be earlier than product production dates.
    - **Limitations**: Data might be consistent but still incorrect or inaccurate. A shipping date could be later than a production date and still be wrong.
- Data structure
    - **Purpose**: Check that the data follows or conforms to a set structure.
    - **Example**: Web pages must follow a prescribed structure to be displayed properly.
    - **Limitations**: A data structure might be correct with the data still incorrect or inaccurate. Content on a web page could be displayed properly and still contain the wrong information.
- Code validation
    - **Purpose:** Check that the application code systematically performs any of the previously mentioned validations during user data input.
    - **Example:** Common problems discovered during code validation include more than one data type allowed, data range checking not done, or ending of text strings not well defined.
    - **Limitations:** Code validation might not validate all possible variations with data input.

# Share data through the art of visualization

## Effective data visualizations

A data visualization, sometimes referred to as a data viz, allows analysts to properly interpret data. A good way to think of data visualization is that it can be the difference between utter confusion and really grasping an issue. Creating effective data visualizations is a complex task; there is a lot of advice out there, and it can be difficult to grasp it all.

In this reading, you are going to learn some tips and tricks for creating effective data visualizations. First, you'll review two frameworks that are useful for thinking about how you can organize the information in your. Second, you'll explore pre-attentive attributes and how they can be used to affect the way people think about your visualizations. From there, you'll do a quick review of the design principles that you should keep in mind when creating your visualization. You will end the reading by reviewing some practices that you can use to avoid creating misleading or inaccurate visualizations.

### McCandless method

- **Information**: the data you are working with
- **Story**: a clear and compelling narrative or concept
- **Goal**: a specific objective or function for the visual
- **Visual** form: an effective use of metaphor or visual expression

## Correlation and causation

Correlation in statistics is the measure of the degree to which two variables move in relationship to each other. An example of correlation is the idea that `as the temperature goes up, ice cream sales also go up`. It is important to remember that correlation doesn't mean that one event causes another. But, it does indicate that they have a pattern with or a relationship to each other. If one variable goes up and the other variable also goes up, it is a positive correlation. If one variable goes up and the other variable goes down, it is a negative or inverse correlation. If one variable goes up and the other variable stays about the same, there is no correlation.

Causation refers to the idea that an event leads to a specific outcome. For example, `when lightning strikes, we hear the thunder`. The sound wave is caused by the air heating and cooling from the lightning strike. Lightning causes thunder.

![Examples of correlation and causation](https://github.com/x-square/visual-resources/blob/main/correlation-causation.png?raw=true 'Examples of correlation and causation')

When you make conclusions from data analysis, you need to make sure that you don't assume a causal relationship between elements of your data when there is only a correlation. When your data shows that outdoor temperature and ice cream consumption both go up at the same time, it might be tempting to conclude that hot weather causes people to eat ice cream. But, a closer examination of the data would reveal that every change in temperature doesn't lead to a change in ice cream purchases. In addition, there might have been a sale on ice cream at the same time that the data was collected, which might not have been considered in your analysis.

For example, pellagra is a disease with symptoms of dizziness, sores, vomiting, and diarrhea. In the early 1900s, people thought that the disease was caused by unsanitary living conditions. Most people who got pellagra also lived in unsanitary environments. But, a closer examination of the data showed that pellagra was the result of a lack of niacin (Vitamin B3). Unsanitary conditions were related to pellagra because most people who couldn't afford to purchase niacin-rich foods also couldn't afford to live in more sanitary conditions. But, dirty living conditions turned out to be a correlation only.

## The wonderful world of visualizations

- **Line chart** is used to track changes over short and long periods of time. When smaller changes exist, line charts are better to use than bar graphs. Line charts can also be used to compare changes over the same period of time for more than one group.
- **Column charts** e.g. bar chart use size to contrast and compare two or more values, using height or lengths to represent the specific values.
- **Heatmaps** also use color to compare categories in a data set. They are mainly used to show relationships between two variables and use a system of color-coding to represent different values. The following heatmap plots temperature changes for each city during the hottest and coldest months of the year.
- **Pie chart** is a circular graph that is divided into segments representing proportions corresponding to the quantity it represents, especially when dealing with parts of a whole.
- **Scatter plots** show relationships between different variables. Scatter plots are typically used for two variables for a set of data, although additional variables can be displayed.
- **Distribution graph** e.g. histogram displays the spread of various outcomes in a dataset.

Meaningful patterns can take many forms, such as:

- **Change** is a trend or instance of observations that become different over time. A great way to measure change in data is through a line or column chart.
- **Clustering** is a collection of data points with similar or different values. This is best represented through a distribution graph.
- **Relativity** is an observation considered in relation or in proportion to something else. You have probably seen examples of relativity data in a pie chart.
- **Ranking** is a position in a scale of achievement or status. Data that requires ranking is best represented by a column chart.
- **Correlation** shows a mutual relationship or connection between two or more things. A scatter plot is an excellent way to represent this type of data pattern.

## Data grows on decision trees

A decision tree is a decision-making tool that allows you, the data analyst, to make decisions based on key questions that you can ask yourself. Each question in the visualization decision tree will help you make a decision about critical features for your visualization. Below is an example of a basic decision tree to guide you towards making a data-driven decision about which visualization is the best way to tell your story. Please note that there are many different types of decision trees that vary in complexity, and can provide more in-depth decisions.

![Best way to represent data](https://github.com/x-square/visual-resources/blob/main/data-dicision-tree.png?raw=true 'Best way to represent data')

Start off by evaluating the type of data you have and go through a series of questions to determine the best visual source:

- Does your data have only one numeric variable?
- Are there multiple datasets?
- Are you measuring changes over time?
- Do relationships between the data need to be shown?

## Principles of design

There are nine basic principles of design that data analysts should think about when building their visualizations.

![Nine principles of design](https://github.com/x-square/visual-resources/blob/main/design-principles-nine.png?raw=true 'Nine principles of design')

`Any questions, please reach out!`

Chiawei Wang, PhD\
Data & Product Analyst\
<chiawei.w@outlook.com>
