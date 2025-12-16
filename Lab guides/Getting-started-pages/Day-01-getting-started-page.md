# Microsoft Fabric: Real Time Analytics - Day 1

### Overall Estimated Duration: 4 Hours

## Overview

In this lab, you will get hands-on experience setting up a Microsoft Fabric Real-Time Analytics environmentand working end to end with streaming and event-based data. You will learn how to configure your environment, ingest data through the Real-Time hub, transform incoming events, and publish an event stream for downstream analytics. The lab also covers creating KQL queries to explore and analyze the data, enabling you to work effectively with real-time data flows in Fabric.

By completing this lab, learners will gain an understanding of how to build real-time analytics solutions in Microsoft Fabric, including creating Real-Time dashboards for visual exploration, generating **Power BI reports from KQL queries, and setting up alerts on event streams to proactively monitor data changes. Learners will also understand how to connect streaming data to interactive visualizations, enabling timely insights and data-driven decision-making.

## Objective

By the end of this lab, participants will be able to:

- **Set up a Fabric-enabled Power BI workspace** to support real-time analytics and KQL database workloads.

- **Create and manage a KQL database** within Microsoft Fabric to store and analyze streaming and event-based data.

- **Ingest data using the Real-Time hub** and **publish event streams** to enable real-time data processing.
  
- **Transform incoming events** to prepare data for querying and visualization.
  
- **Create and run KQL queries using a KQL Queryset** to explore and analyze data efficiently.
  
- **Manage the KQL database using control commands and policies** to configure behavior, performance, and governance.
  
- **Build and explore Fabric Real-Time dashboards** to visualize streaming data and gain immediate insights.

- **Create Power BI reports from KQL queries** to extend real-time analysis into interactive business reports.
  
- **Set alerts on event streams** to proactively monitor data changes and respond to critical conditions.

## Prerequisites

Participants should have:

- Basic understanding of Power BI, Fabric, data modeling concepts, and report building.

## Explanation of Components

The architecture for this lab involves the following key components:

1. **Fabric-enabled Power BI Workspace:** A centralized workspace that hosts and manages all Microsoft Fabric real-time analytics assets.
2. **KQL Database:** A high-performance database optimized for storing and querying streaming and event-based data using KQL.
3. **Real-Time Hub:** The entry point in Fabric for discovering, connecting, and ingesting real-time data sources.
4. **Event Stream:** A pipeline that routes real-time data from sources to destinations with optional transformations.
5. **Event Transformation:** A process to filter, enrich, and reshape streaming data before analysis or storage.
6. **KQL Queryset:** An interactive environment for writing and executing KQL queries against a KQL database.
7. **Control Commands and Policies:** Administrative configurations used to manage ingestion, retention, security, and performance of a KQL database.
8. **Fabric Real-Time Dashboard:** A live dashboard that visualizes streaming data for instant insights and monitoring.
9. **Visual Exploration in Real-Time Dashboards:** Interactive analysis of live data through filters, visuals, and real-time updates.
10. **Power BI Report from KQL Query:** A Power BI report built on KQL queries to extend real-time insights into rich analytics.
11. **Alerts on Event Streams:** Automated notifications triggered when defined conditions are met in streaming data.
12. **Workspace Cleanup:** Ensures resources are deleted after learning activities. Helps maintain a cost-efficient environment.

## Architecture

In this lab, you will use **Microsoft Fabric Real-Time Analytics** to build an end-to-end streaming and analytics workflow that enables real-time data ingestion, processing, analysis, visualization, and alerting. The process begins by setting up a **Fabric-enabled Power BI workspace** and creating a **KQL database** to serve as the analytical store for event and streaming data.

You will ingest live data through the **Real-Time hub**, publish and manage **event streams**, and apply **event transformations** to clean, filter, and enrich data as it flows through the pipeline. The transformed events are ingested into the KQL database, where you will use **KQL Querysets** to run powerful KQL queries and explore both real-time and historical data.

Finally, you will create **Fabric Real-Time dashboards** to visualize streaming insights, build **Power BI reports from KQL queries** for interactive business reporting, and configure **alerts on event streams** to proactively monitor conditions and respond to critical events—demonstrating a complete, production-ready real-time analytics architecture in Microsoft Fabric.

## Getting Started with the Lab
 
Once the environment is provisioned, a virtual machine (LabVM) and lab guide will be loaded in your browser. Use this virtual machine throughout the workshop to perform the lab. You can see the number on the bottom of the Lab guide to switch to different exercises in the lab guide.
 
## Accessing Your Lab Environment
 
Once you're ready to dive in, your virtual machine and **Guide** will be right at your fingertips within your web browser.
 
   ![](../Use%20Case%2001/media/Intro-00.png)

### Virtual Machine & Lab Guide
 
Your virtual machine is your workhorse throughout the workshop. The lab guide is your roadmap to success.
 
## Exploring Your Lab Resources
 
To get a better understanding of your lab resources and credentials, navigate to the **Environment** tab.
 
   ![](../Use%20Case%2001/media/Intro-01.png)
 
## Utilizing the Split Window Feature
 
For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the top right corner.
 
![](../Use%20Case%2001/media/Intro-02.png)
 
## Managing Your Virtual Machine
 
Feel free to start, stop, or restart your virtual machine as needed from the **Resources** tab. Your experience is in your hands!
 
![](../Use%20Case%2001/media/Intro-03.png)

## Lab Guide Zoom In/Zoom Out

To adjust the zoom level for the environment page, click the **A↕ : 100%** icon located next to the timer in the lab environment.

   ![](../Use%20Case%2001/media/Intro-04.png)
 
## Let's Get Started with Microsoft Portal
 
1. On your virtual machine, open the **Microsoft Edge**.
 
    ![](../Use%20Case%2001/media/Intro-05.png)
 
2.  In a new tab, navigate to the **Microsoft Fabric** portal by copying and pasting the following URL into the address bar:

      ```
      https://app.fabric.microsoft.com
      ```

3. On the **Enter your email, we'll check if you need to create a new account** tab, you will see the login screen, in that enter the following email/username, and click on **Submit**.

    - **Email/Username:** <inject key="AzureAdUserEmail"></inject>
 
        ![](../Use%20Case%2001/media/GS5.png)
 
4. Next, provide your password:
 
   - **Password:** <inject key="AzureAdUserPassword"></inject>
 
        ![](../Use%20Case%2001/media/Intro-07.png)

5. First-time users are often prompted to Stay Signed In. If you see any such pop-up, click on **No**.
   
    ![](../Use%20Case%2001/media/Intro-08.png)

6. On Microsoft Fabric (Free) license assignment dialog appears, click **OK** to proceed.

    ![01](./media/Intro-09.png)

7. You will be navigated to the **Microsoft Fabric page**.

    ![01](./media/Intro-10.png)

## Support Contact

The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:

- Email Support: cloudlabs-support@spektrasystems.com
- Live Chat Support: https://cloudlabs.ai/labs-support

Now, click on **Next** from the lower right corner to move on to the next page.
 
![](../Use%20Case%2001/media/Intro-11.png)

## Happy Learning!!
