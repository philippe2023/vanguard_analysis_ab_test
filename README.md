# Project overview
This study aimed to test whether a redesigned user interface (UI), featuring modern, intuitive elements and in-context prompts (cues, messages, hints), would improve user experience and increase the completion rates of an online process. This process involved several steps, culminating in the final confirmation page. The experiment employed A/B testing between two groups:

    Control Group: Clients interacting with the traditional online process.
    Test Group: Clients using the new, modern interface.
The objective was to assess if the redesigned interface led to higher completion rates, indicating a smoother and more user-friendly experience.

# Questions 
The study was based on these three questions:
1. What is the completion rate of the new design compared to the old one?
3. How much time do users spend on each step in the process for the Test and Control groups?
4. What are the error rates for each group?

# Dataset 
The analysis utilized three key datasets:

1. Client Profiles (df_final_demo : https://github.com/data-bootcamp-v4/lessons/blob/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_demo.txt): Contains demographic information such as age, gender, and account details. 
2. Digital Footprints (df_final_web_data): Contains a trace of client interactions online, split into two parts (pt_1 : https://github.com/data-bootcamp-v4/lessons/blob/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_web_data_pt_1.txt and pt_2: https://github.com/data-bootcamp-v4/lessons/blob/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_web_data_pt_2.txt), which need to be merged. 
3. Experiment Roster (df_final_experiment_clients : https://github.com/data-bootcamp-v4/lessons/blob/main/5_6_eda_inf_stats_tableau/project/files_for_project/df_final_experiment_clients.txt): A list identifying which clients participated in the experiment.

## Main dataset issues
- Data Imbalance:
The Control and Test groups had varying sample sizes, which made direct comparisons more challenging and required careful statistical methods to ensure valid results.
- Complex User Behavior:
Tracking user progress through multiple steps introduced complexity, particularly when analyzing users who revisited steps or spent different amounts of time on each step. This added a layer of difficulty when interpreting user interaction data.
- Error Rates & Variations:
Identifying and interpreting error rates across different steps and variations was challenging. It required special attention to ensure accurate analysis, as even minor discrepancies in error rates could skew the results.

# Conclussions
The results of the experiment indicate that the new design implemented for the Test group led to improvements in both time spent and completion rates, particularly for younger users who found the interface more intuitive. However, challenges remain for older users, as they experienced higher error rates and spent more time on each step of the process. This suggests that while the redesigned interface has potential, it is not universally effective for all user demographics. Addressing the specific difficulties encountered by older users will be key to fully realizing the benefits of the new interface.

# Next steps
- Focus on Key Steps with Higher Error Rates: Identify the steps in the process where older users are encountering the most errors. These steps may require redesign or clearer instructions to help users navigate them more easily.
- Provide Additional Support for Older or First-Time Users: Consider introducing help features such as tooltips, tutorials, or in-context assistance specifically targeted at older users or those unfamiliar with the process.
- Conduct Usability Testing Focused on Older Demographics: Carry out further testing and feedback sessions specifically with older users to better understand their pain points and adjust the UI accordingly.
- Implement a Personalized UI: Based on the age or experience level of users, provide different versions or levels of UI support. Younger users might prefer a streamlined experience, while older users might benefit from a more guided approach.
- Monitor Post-Implementation Metrics: After making the changes, continue tracking completion rates, time spent, and error rates to ensure the improvements are effective and the user experience is enhanced for all age groups.
