@lab.Title

Login to your VM with the following credentials...

**Username: +++@lab.VirtualMachine(WRK523).Username+++**

**Password: +++@lab.VirtualMachine(WRK523).Password+++**

<br>
***



## Microsoft Purview DSPM for Ai Data Risk Assessment

1. Launch Edge and go to 'https://Purview.microsoft.com' 
2. Click the **Solutions** button on the left navigation rail. 
3. Click on **DSPM for AI** from the Solutions button.
4. Click on **Data risk assessments** at the bottom. 
5. The top section will be blank, but by launching this Section you have triggered the default assessment to run.  It will take up to 4 days to populate the default report. 
6. Default assessment runs every week on the top 100 SharePoint sites based on how many times the sites are accessed. 
7. Click on **Create custom assessment**
8. In the basic details tab, give your assessment a meaningful name and description. 
9. Click **Next**
10. In the Add users tab, click on the **Include specific** box and then click **Add users**
11. in the Add users or groups flyout, find Adele Vance, check the box next to her name and click **Add**
12. In the Add data sources to assess tab, Select both SharePoint and OneDrive and click **Next**
13. For Review and run tab, click on **Save and run**
14. Click **Done** on the data assessment successfully created page.


## Data Loss Prevention for Copilot

1. Launch Edge and go to 'https://Purview.microsoft.com' 
2. Select **Data Loss Prevention** in the Solutions, and click on **Policies**
3. Then click on **+ Create policy** to create a new DLP for Copilot policy to block Microsoft 365 Copilot and Agents in Microsoft 365 processing any document labeled with a specific sensitivity label, such as Highly confidential.
4. Choose **Data stored in connected sources**, and click **Next**
5. Click **Custom** under Categories, and then click **Custom Policy** under Regulations,  click the **Next** at the bottom. 
6. Give your policy a name of your chosing and click **Next**
7. We will not be assigning Admin Units, so simply click **Next**
8. On the "Choose where to apply the policy" page, select **Microsoft 365 Copilot** and then click **Next**
9. On "Define policy settings". Select **Create or customize advanced DLP rules** and click **Next**
10. On "Customize advanced DLP rules, Click on **+ Create Rule**
11. Fill in a Name for the rule that makes sense.  
12. Under "Conditions" click **+ Add Condition** and then select **Content contains**
13. You may optionally name the Group, and then click **Add** under **Content Contains**, then click **Sensitivity labels.**
14. Select the sensitivity label you want M365 Copilot and agents to not process, in this case we're going to choose **Highly Confidential** and click **Add.** 
15. Back in the Create rule, we are going to scroll down to Actions and click on **+ Add an action**. and then select **Prevent Copilot from processing content.**
16. Scroll to the bottom and optionally you can turn on alerts. 
17. Click on **Save**
18. Back on the "Customize advanced DLP rules" page, Double check your advanced DLP rule is correct and then click **Next**
19. On the "Policy mode" page Select **Turn the policy on immediately** and click **Next**
20. On the "Review and finish" page, make sure the policy is correctly named and the confirm the settings are correct.. then click **Submit**
21. Finally on the New policy created page click **Done**


**✅ DLP policy created to exclude Highly Confidential items from Copilot processing.**

 
## Information Rights Management: Risky AI Usage Policy

1. Launch Edge and go to 'https://Purview.microsoft.com' 
2. Click the **Solutions** button on the left navigation rail. 
3. Select **Insider Risk Management** from the **Solutions** button, and go to the **Policies** tab.
4. Click on **+ Create policy** to create a new Risky AI usage policy for Microsoft 365 Copilot and Agents in Microsoft 365.
5. Select **Custom policy.**
6. On the "Choose a policy template" page, Select the **Risky AI usage** template and click **Next**.
7. Type in a name for your policy and click **Next**.
8. On "Choose users, groups & adaptice scopes", Select** All users, groups, and adaptive scopes**, and click **Next**.
9. We will not be excluding users and groups so just click **Next**.
10. On "Decide whether to prioritize content", Select **I don't want to prioritize content right now** and click **Next**.
11. On "Choose triggering event for this policy", Click **Select all** to select all triggering events for this policy and click **Next**.
12. On "Choose thresholds for triggering events", Click **Apply built-in thresholds** and click **Next**.
13. On "Indicators", Click **Turn on Indicators** in the top box, and then Select **all Indicators**
14. Below expand "Generative AI Apps" and click **Select all** under "Microsoft Copilot experiences" and click **Next**
15. On "Detection Options", everythign should be selected, Click **Next.**
16. On "Choose threshold type for indicators", Click **turn on analytics**, then Select **Apply thresholds provided by Microsoft** and click **Next**.
17. On "Review settings and finish" confirm everything looks correct and click **Submit**
18. On "Your policy was created", click **Done**.

**✅ Risky AI Usage Policy successfully created.**

## Communication Compliance policy to detect inappropriate messaging 

1. Launch Edge and go to 'https://Purview.microsoft.com' 
2. Click the **Solutions** button on the left navigation rail. 
3. Select **Communication Compliance** from the **Solutions** button and click on the **Policies** tab.
4. Click on the **X** to close out any information boxes that pop up. 
5. Click **+ Create policy** to create a new policy to detect noncompliant content within Microsoft 365 Copilot and Agents in Microsoft 365.
6. Select **custom policy**.
7. Name your policy and click **Next**.
9. Select **All users**, under Reviewers type **"Admin"** in the search box and select **"MOD Administrator"**, then click **Next**
10. On "Choose locations to detect communications" Select **+ Generative AI** make sure **M365 Copilot** is selected and click **Add**  click **Next**.
11. On "Choose conditions and review percentage" Click on **+ Add condition**, and select **Content matches trainable classifiers**.
12. Click **Add** under **Content matches trainable classifiers** and select **+ Trainable classifiers**.
13. Select the trainable classifiers you wish to detect and click **Add**.
14. Click **Next**.
15. Review and finish by clicking **Create policy** and click **Done**

**✅ Communication Compliance Policy created to detect inappropriate messaging.**
