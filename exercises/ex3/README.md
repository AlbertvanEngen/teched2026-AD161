# Exercise 3 - Build, Test, Deploy and Operate an agentic solution with Joule Studio

In this exercise, we will create a soluton that would comprise of an agent and mcp servers that would interact with S/4HANA Public Cloud to retrieve information on products. The solution would then be tested, deployed & monitored. You will also interact with the agent that you created in Joule Work Conversations. 

## Exercise 3.1 Create a solution via Joule Studio

After completing these steps you would have created a solution that comprise of an agent and mcp servers that would interact with S/4HANA Public Cloud to retrieve information on products. 

1. Log-in to Joule Work & Navigate to Joule Studio
   <br>![](./images/1.JouleStudio.png)

2. Create a new Solution
    - Name: Read products from S/4HANA
    - Description: An AI agent that enables Sales Representatives to ask natural language questions about product master data from SAP S/4HANA and receive instant, accurate answers.
    - Ensure that "Quick Create" is not checked
    <br>![](./images/2.CreateANewSolution.png)

3. Interact with the Joule Studio Agent and clarify questions to provide additional context and information to provide enough context for creation of the intent

    - Which types of product information should Sales Representatives be able to ask about? **Specify**: `Basic Product Details`
      <br>![](./images/3.ClarifyingQuestions-1.png)

    - What is the main pain point that drives this need? **Specify**: `Sales reps waste time switching between SAP screens to find the product`
      <br>![](./images/4.ClarifyingQuestions-2.png)
    
    - What does success look like? **Specify**: `Reduce time from to find product info (from 5 mins to under 30 seconds)`

    - Do you have a baseline? **Specify**: `Baseline is 5 mins`

    - What target response time? **Specify**: `Under 30 seconds - within 3 months`

    - Does this look correct? **Specify**: `Confirm`

    - Please review the summary above. Does everything look correct, or would you like to adjust anything before I write the intent document? **Specify**: `Confirm proceed with intent.md`
      <br>![](./images/9.ClarifyingQuestions-7.png)

4. Interact with the Joule Studio Agent to create the Product Requirements Document

    - Would you like to proceed to generating the Product Requirements Document (PRD), which will turn this intent into a detailed set of requirements for building the agent? **Specify**: `Yes`
      <br>![](./images/10.GeneratePRD.png)

    - Does this PRD plan look correct? Shall I proceed with writing the full document? **Specify**: `Confrim - write PRD`

5. Interact with the Joule Studio Agent to create the Specification that explains how the intent and PRD can be realized 
    - The natural next step is the Specification phase, where the PRD is turned into a detailed, actionable build checklist. Would you like to proceed? **Specify**: `Proceed with Specification`
      <br>![](./images/12.CreateSpec.png)

6. Interact with Joule Studio Agent to build the solution based on the Specification, PRD and Intent

    - You can review and adjust the spec files before building. When ready, say "execute specification/specification.md" to start the implementation. **Specify**: `execute specification/specification.md`
      <br>![](./images/13.ExecuteSpec.png)

## Exercise 3.2 Observe the artifacts created and explore the tests generated

After completing these steps you will have learnt more about the agent and mcp server created and the generated automated tests

1. Navigate to the Solution Artifacts and Select the agent
    <br>![](./images/14.AgentDetails-LLMModel.png) 
    <br>![](./images/15.AgentDetails-MCP.png) 

2. Navigate to Solution Artifacts and Select the mcp server
    <br>![](./images/16.MCPDetails.png) 

3. Navigate to Testing > Overview
    <br>![](./images/17.UnitTests.png) 

4. Navigate to File tree and observe the files created for the solution

## Exercise 3.3 Test your Agent

After completing these steps you will have learnt how to test your agent that does not hit the backend systems

1. Navigate to Preview > Agent
    
2. Interact with your agent with a few questions and observe it's response
    - List 5 products
      <br>![](./images/18.TestAgent-1.png) 

    - List top 5 products sold last month
      <br>![](./images/19.TestAgent-2.png)  

## Exercise 3.4 Deploy your Agent

After completing these steps you will learn how to deploy and understand the status of your solution and artifacts within the solution

1. Interact with the Joule Studio Agent to deploy the solution	
    - When you're ready to deploy, just say "deploy". **Specify**: `deploy`
      <br>![](./images/20.DeploySolution.png)  

2. Navigate to Manage > Overview to understand the status of the solution and agent and wait for the deployment to complete
      <br>![](./images/21.SolutionStatus.png)  

3. Navigate to Manage > Deployment History to understand the state of the current and past deployments
      <br>![](./images/22.DeploymentHistory.png)  

## Exercise 3.5 Try out your Agent with Joule Studio and Joule Work Convesations

After completing these steps you will learn test your agent as an end user. 

1. Ask the instructor to grant you access to try out your agent

2. Navigate to Manage > Overview and select Agent > 'Try Now'
      <br>![](./images/23.TryOut-AfterDeployment.png)  

3. Interact with your agent with a few questions and observe it's response
    - List 5 products

    - List top 5 products sold last month

3. Navigate to Conversations and interact with you with the following conversations and observe it's response

    - Use @product-master-data-agent (agent name) to `List 5 products`

    - Use @product-master-data-agent (agent name) to `List top 5 products sold last month`

    ```
    Note: you can get the agent name from the Solution > Manage > Overview
    ```
      <br>![](./images/24.AgentName.png)

## Exercise 3.6 Monitor your Agent

After completing these steps you will learn how your agent is performing in the real world. You can monitor and understand it's success rate and get details of each execution.

1. Navigate to Manage > Monitoring & Analytics > roduct-master-data-agent > Monitoring

2. Navigate to Manage > Monitoring & Analytics > roduct-master-data-agent > Traces

3. Navigate to Manage > Monitoring & Analytics > roduct-master-data-agent > Monitoring > Explore a single trace


## Summary

You've now created a soltion comprising of an agent and mcp server. You now understand the different steps, the lifecycle and are in a position to deploy, run and monitor the solution and agent. 

Continue to - [Exercise 4 - Push your agentic solutions to git and promote to production](../ex4/README.md)