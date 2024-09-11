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

## Solutions for the dataset issues
- Handling Data Imbalance:
To mitigate the impact of sample size differences, statistical methods such as weighted analysis, stratified sampling, or normalization techniques were applied. These adjustments ensured that the smaller group did not disproportionately affect the outcome.
- Addressing Complex User Behavior:
A detailed tracking mechanism was implemented to account for step reversions and variations in time spent. This included creating user journey segments and incorporating advanced metrics to evaluate different types of user behavior effectively.
- Managing Error Rates & Variations:
To accurately interpret error rates, we introduced error tracking at each individual step of the process and applied statistical tests to determine if differences in error rates between groups were significant. Careful attention was paid to avoid overinterpreting minor variations.

# Conclussions
The study specifically measured completion rates (whether users reached the final confirmation step), time spent on each step, and error rates (instances of users reverting to previous steps). Both groups were segmented by gender/age and tenure to ensure we accounted for various behavioral factors.

# Next steps
...
