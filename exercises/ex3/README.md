# Exercise 3 - Build, Test, Deploy and Operate an agentic solution with Joule Studio

In this exercise, we will create a soluton that would comprise of an agent and mcp servers that would interact with S/4HANA Public Cloud to retrieve information on products. The solution would then be tested, deployed & monitored. You will also interact with the agent that you created in Joule Work Conversations. 

## Exercise 2.1 Create a solution via Joule Studio

After completing these steps you would have created a solution that comprise of an agent and mcp servers that would interact with S/4HANA Public Cloud to retrieve information on products. 

1. Log-in to Joule Work & Navigate to Joule Studio

2. Create a new Solution
a. Name: Read products from S/4HANA
b. Description: An AI agent that enables Sales Representatives to ask natural language questions about product master data from SAP S/4HANA and receive instant, accurate answers.
c. Ensure that "Quick Create" is not checked

3. Interact with the Joule Studio Agent and clarify questions to provide additional context and information to provide enough context for creation of the intent

a. Which types of product information should Sales Representatives be able to ask about? Specify: Basic Product Details

b. What is the main pain point that drives this need? Specify: Sales reps waste time switching between SAP screens to find the product

c. What does success look like? Specify: Reduce time from to find product info (from 5 mins to under 30 seconds)

d. Do you have a baseline? Specify: Baseline is 5 mins

e. What target response time? Specify: Under 30 seconds - within 3 months

f. Does this look correct? Specify: Confirm

g. Please review the summary above. Does everything look correct, or would you like to adjust anything before I write the intent document? Specify: Confirm — proceed with intent.md

4. Interact with the Joule Studio Agent to create the Product Requirements Document

a. Would you like to proceed to generating the Product Requirements Document (PRD), which will turn this intent into a detailed set of requirements for building the agent? Specify: Yes

b. Does this PRD plan look correct? Shall I proceed with writing the full document? Specify: Confrim - write PRD

5. Interact with the Joule Studio Agent to create the Specification that explains how the intent and PRD can be realized 
a. The natural next step is the Specification phase, where the PRD is turned into a detailed, actionable build checklist. Would you like to proceed? Specify: Proceed with Specification

6. Interact with Joule Studio Agent to build the solution based on the Specification, PRD and Intent

a. You can review and adjust the spec files before building. When ready, say "execute specification/specification.md" to start the implementation. Specify: execute specification/specification.md

## Exercise 2.2 Observe the artifacts created and explore the tests generated

After completing these steps you will have learnt more about the agent and mcp server created and the generated automated tests

1. Navigate to the Solution Artifacts and Select the agent

2. Navigate to Solution Artifacts and Select the mcp server

3. Navigate to Testing > Overview

4. Navigate to File tree and observe the files created for the solution

## Exercise 2.3 Test your Agent

After completing these steps you will have learnt how to test your agent that does not hit the backend systems

1. Navigate to Preview > Agent

2. Interact with your agent with a few questions and observe it's response
a. List 5 products

b. List top 5 products sold last month

## Exercise 2.4 Deploy your Agent

After completing these steps you will learn how to deploy and understand the status of your solution and artifacts within the solution

1. Interact with the Joule Studio Agent to deploy the solution	
a. When you're ready to deploy, just say "deploy". Specify: deploy

2. Navigate to Manage > Overview to understand the status of the solution and agent and wait for the deployment to complete

3. Navigate to Manage > Deployment History to understand the state of the current and past deployments

## Exercise 2.5 Try out your Agent with Joule Studio and Joule Work Convesations

After completing these steps you will learn test your agent as an end user. 

1. Ask the instructor to grant you access to try out your agent

2. Navigate to Manage > Overview and select Agent > 'Try Now'

3. Interact with your agent with a few questions and observe it's response
a. List 5 products

b. List top 5 products sold last month

3. Navigate to Conversations and interact with you with the following conversations and observe it's response
a. List 5 products

b. List top 5 products sold last month

## Exercise 2.6 Monitor your Agent

After completing these steps you will learn how your agent is performing in the real world. You can monitor and understand it's success rate and get details of each execution.

1. Navigate to Manage > Monitoring & Analytics > Agent > Monitoring

2. Navigate to Manage > Monitoring & Analytics > Agent > Traces

3. Navigate to Manage > Monitoring & Analytics > Agent > Monitoring > Explore a single trace


## Summary

You've now created a soltion comprising of an agent and mcp server. You now understand the different steps, the lifecycle and are in a position to deploy, run and monitor the solution and agent. 

Continue to - [Exercise 4 - ](../ex4/README.md)
