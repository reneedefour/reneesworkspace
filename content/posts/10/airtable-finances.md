---
title: "How I Track and Plan Personal Finances in Airtable"
date: 2022-03-18T20:14:51-04:00
draft: false
tags: ["organization", "personal finances"]
categories: ["digital workspace"]
cover:
    image: posts/10/10-transactions.png
---

## Why I track my finances manually
- There are many apps available to track expenses and I’m almost certain that this is the most convenient and accurate tool if you live in a country where the app is compatible with the banks that you use. Because I live in Trinidad, many, if not all of the apps that I’ve come across, do not allow connections with our local banks.
- Entering every expense and keeping to a regular “base update routine” has helped me to be more mindful of my spending. While I’m not a big spender generally, I tend to spend more than I should on things like food, in particular, sushi. Knowing and seeing that I’ve already spent x amount on sushi for the month, I tend to think twice before placing another order.

## What I need in a finance planner
- Tracking of: income, expenses, savings, projects and transactions involving other persons.
- Budget
- Logging of recurring bills
- Asset tracker
- Monthly review of total income, expenses and savings

## To Note
- This base is built specifically for my needs and therefore it’s certainly not ideal for everyone. Some of the tables, like budget for example, do not actually work as a budget in the traditional sense and are still being planned out.
- I built this base and started using it at the beginning of this month (March, 2022) and so, as I continue to use it, I will be able to tweak and improve on this initial system. This is a work in progress.
- The online Airtable community is quite robust and extremely helpful. By searching for ‘expenses’ or ‘budget’ in the Airtable Universe, I was able to see bases built by other people and to learn how Airtable works.
- Currency: Trinidad and Tobago Dollar (TTD)

## Base Tour
The base currently consists of 8 tables: transactions, budget, recurring bills, debtors, projects, assets, monthly review and notes.

### 💵 All Transactions
This is the main table which houses income, expenses and interpersonal transactions. The master view shows all fields (columns) of the transactions table.

![Transactions](/posts/10/10-transactions.png)

#### This Month
- Shows records (rows) grouped by type of transaction — income, expenses, upcoming expenses and savings.
- Sorted by date field
- Filtered by a lookup field titled month status which shows only the record from the monthly review table whose status is tagged with ‘ 📌 This Month’. This field is hidden in this view.

![This month](/posts/10/10-thismonth.png)

#### Monthly Expenses
- Shows records grouped by month which is a linked field connecting the Monthly Expenses view with the records of Monthly Review.
- Filtered by type — expenses.

![Monthly expenses](/posts/10/10-expenses.png)

#### Upcoming Expenses
- Shows records grouped by month and filtered by type — upcoming expenses.

#### Moving Out
- Shows records grouped by type — upcoming expense
- Filtered by projects which is a linked field connecting the Moving Out view with the records of Monthly Review. Filter shows records where projects contains “Moving”.
- This is only here because I’m currently in the process of moving out. After, I can view these expenses under the Projects table.

#### Debt
- Tracks money that I owe to persons (immediate family and partner).
- Grouped by person
- Fields: amount, transaction date, paid checkbox, date paid and others related to the transaction.

#### Transactions
- Tracks money owed to me
- Filtered and grouped by debtor field
- Split cost formula field divides the amount number in two

![Transactions 2](/posts/10/10-transactions2.png)

### 💰 Budget
The budget is a work in progress. Right now, it serves as a sort of checklist view so that I know which expenses are budgeted vs. those that I’ve already paid. This will become more useful from next month as I will begin to use the majority of these fields after moving. For now, I can easily see what my projected budget will look like. I don’t actually add records to this table, these are added in the ‘Recurring Bills’ table.

![Budget](/posts/10/10-budget.png)

### 🔃 Recurring Bills
The idea here is to copy and paste these recurring monthly expenses when I do my budgeting for the next month. This way, I have a log of the amounts that I’ve paid on a monthly basis for each expense as the table is grouped by month. I will be able to post an update on how this works practically at the end of April 2022.

I’m working on an automation to update the 💰 Budget status to paid based on triggers in the Recurring Bills table but I’ll definitely need more time to set this up properly (if it’s possible without being too clunky).

![Recurring bills](/posts/10/10-recurring.png)

### 👤 Debtors
This is linked to the transactions view and contains names of persons who owe money to me, as well as the amount, previous payments, transaction date and the date paid.

### 🏡 Projects
This table has a gallery view which links all expense records tagged with a given project. There is also a rollup field which sums up the total amount of money that I’ve spent on the project.

![Projects](/posts/10/10-projects.png)

### 🏦 Assets
This is a grid view to track investments with the following fields: name, amount, description (e.g. short and long term emergency fund, insurance), provider (bank/financial institution), type (e.g. fixed deposit, mutual fund), start date, interest rate, status (acting, inactive, pending), attachments (for certificates and receipts) and notes.

### 🗓 Monthly Review
Allows me to easily see my total income, expenses and the amount that I have remaining. I think that I should also add a field for total savings here as well, but this view gives an overall summary of the month.

![Monthly review](/posts/10/10-monthlyrev.png)

📝 Notes
In notes, I have random things that I want to view or calculate. I’m thinking that I should create a new base for this purpose as it won’t be very practical to either add additional tables to this base.

![Notes](/posts/10/10-notes.png)

## All done
That’s it. It’s not perfect and there are quite a few parts that I would like to adjust but for now I’m enjoying the process of building it out. In addition to making this base more efficient, I think it would be fun to build this in Notion as well. I’d love to know if anyone else is using Airtable to plan their personal finances and, as you can tell, I love screenshots so feel free to message on [twitter](https://twitter.com/reneedefour) or leave a comment if you have any suggestions!