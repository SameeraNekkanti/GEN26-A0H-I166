# Genesis 2026: Ideathon
## 12. Research Basis

We reviewed the literature using Scopus AI and LeapSpace across four searches: (1) mental health of college students, (2) students expressing emotions to chatbots, (3) privacy risks of emotional-support chatbots, and (4) campus mental health apps with counsellor risk triage. This evidence shaped each HAVEN design decision.

### 12.1 What the research shows

**The problem is large and persistent.**
- Studies report depression and anxiety in roughly 28% to over 60% of college students, and suicidal thoughts in about 13% to 19%, including Indian samples (Bhat et al., 2018; Cherian et al., 2025).
- Mason et al. (2025) studied 72,288 first-year students across 18 countries on prevalence, age of onset, and course of mental disorders.
- Zivin et al. (2009) found that about 60% of students with problems at baseline still had them two years later, and fewer than half received treatment. This supports early detection.

**Students turn to chatbots, with mixed results.**
- Students cite accessibility, anonymity, and reduced stigma as reasons to use chatbots (Miqdadi et al., 2025; Zhao et al., 2025).
- Actual use is still low in at least one survey: only 5% of U.S. college students had sought support from a chatbot (Rackoff et al., 2025).
- Most students still prefer human counsellors for trust and serious problems (Miqdadi et al., 2025).

**Chatbots carry privacy and safety risks.**
- Disclosures can be stored, analysed, or shared without the user's full awareness, and many students conflate chatbot empathy with human accountability (Zhang et al., 2026; Croes et al., 2024).
- Anonymity increases comfort in disclosing but may lower vigilance about privacy (Croes et al., 2024).
- Overreliance, reduced human connection, and emotional dependence are documented risks (Al-Zahrani, 2025; Laestadius et al., 2024).
- Visible privacy assurances combined with professional-boundary warnings gave the best-calibrated trust (Zhang et al., 2026).

**Human support works better than pure automation.**
- In a university counselling service, video consultation gave better outcomes and lower dropout than asynchronous online CBT in more severe cases (Mammarella et al., 2024).

**Risk scoring and stepped care are feasible.**
- A freshman screening model sorted students into low (under 6%), moderate (6-65%), and high (over 65%) risk, each linked to a different response (Ma et al., 2026).
- Passive smartphone sensing data can predict stress in university students (Shvetcov et al., 2024).
- Risk scores from smartphone data can be condensed into simple results for counselling centres (Langholm et al., 2023).

**Privacy is both a benefit and a barrier.**
- Students are more willing to use tools that feel confidential, but many raise privacy concerns about apps and data use, and mistrust of the institution can reduce uptake (Melcher & Torous, 2020; Kodish et al., 2023).
- In one student survey, 46.0% had at least one privacy, confidentiality, or data-use concern (Soneson et al., 2025).

### 12.2 How the evidence shaped HAVEN

| Finding | HAVEN design decision |
|---|---|
| Students value anonymity and lower stigma | Anonymous login option, restricted to one college |
| Anonymity can lower privacy vigilance | Visible, plain-language privacy notices and consent screens |
| Privacy assurances plus boundary warnings build calibrated trust | In-app notices that state what HAVEN does and does not do |
| Students trust humans for serious problems; human-supported care retains more users in severe cases | In-app real counsellor, not an AI companion |
| Chatbots risk overreliance and weak crisis handling | AI used only for early-signal detection, with crisis escalation to a human |
| Stepped-care routing by risk level is feasible | Private nudge first, then counsellor, peer, or helpline, with thresholds validated by the campus counsellor |
| Passive sensing predicts stress | On-device sleep and activity signals plus a weekly check-in |
| Privacy concerns and institutional mistrust block uptake | Raw data stays on the phone; never used for grades or discipline; aggregate insights only for groups of 20+ |

### 12.3 Research gap HAVEN addresses

- The search found no single paper on how concerning it is when students express emotions to chatbots without realising the privacy risks. The literature covers these aspects only in parts.
- The search found no completed, well-evaluated campus app that combines private or anonymous disclosure, strong privacy design, risk-based counsellor outreach, and measured real-world outcomes. Most work covers one piece.
- Studies report model performance far more often than what happens after an alert, such as counsellor response time, referral completion, and false alerts. HAVEN's pilot measures exactly these (see Section 10).

### 12.4 References

1. Al-Zahrani, A.M. (2025). Exploring the impact of artificial intelligence chatbots on human connection and emotional support among higher education students. *SAGE Open*. https://doi.org/10.1177/21582440251340615
2. Bhat, S.U., Amaresha, A.C., Kodancha, P., et al. (2018). Psychological distress among college students of coastal district of Karnataka: A community-based cross-sectional survey. *Asian Journal of Psychiatry*.
3. Cherian, A.V., Armstrong, G., Sobhana, H., et al. (2025). Mental health, suicidality, health, and social indicators among college students across nine states in India. *Indian Journal of Psychological Medicine*.
4. Croes, E.A.J., Antheunis, M.L., Van Der Lee, C., De Wit, J.M.S. (2024). Digital confessions: The willingness to disclose intimate information to a chatbot and its impact on emotional well-being. *Interacting with Computers*.
5. Kodish, T., Schueller, S.M., Lau, A.S. (2023). Barriers and strategies to improve digital mental health intervention uptake among college students of color: A modified Delphi study. *Journal of Behavioral and Cognitive Therapy*. https://doi.org/10.1016/j.jbct.2022.12.002
6. Laestadius, L., Bishop, A., Gonzalez, M., et al. (2024). Too human and not human enough: A grounded theory analysis of mental health harms from emotional dependence on the social chatbot Replika. *New Media and Society*.
7. Langholm, C., Alon, N., Perret, S., Torous, J. (2023). Risk scores in digital psychiatry: Expanding the reach of complex smartphone data by condensing it into simple results. *Journal of Behavioral and Cognitive Therapy*. https://doi.org/10.1016/j.jbct.2023.05.004
8. Ma, C.-Z., Xiao, F., Zhang, J., et al. (2026). Predicting psychological risk among college students using the Freshman Entrance Psychological Survey: A machine learning model based on LASSO-logistic regression. *Journal of Affective Disorders*. https://doi.org/10.1016/j.jad.2025.120903
9. Mammarella, S., Giusti, L., Del Vecchio, S., et al. (2024). Psychological distress and academic success: A two-year study comparing the outcome of two online interventions at a university counseling and consultation service in Italy. *Frontiers in Psychiatry*. https://doi.org/10.3389/fpsyt.2024.1427316
10. Mason, A., Rapsey, C., Sampson, N., et al. (2025). Prevalence, age-of-onset, and course of mental disorders among 72,288 first-year university students from 18 countries in the WMH-ICS initiative. *Journal of Psychiatric Research*.
11. Melcher, J., Torous, J. (2020). Smartphone apps for college mental health: A concern for privacy and quality of current offerings. *Psychiatric Services*. https://doi.org/10.1176/APPI.PS.202000098
12. Miqdadi, A.I., Halabi, M.N., Alhadidi, M., et al. (2025). Attitudes toward seeking professional psychological help, self-stigma of seeking help, and preferences for AI mental health chatbots vs. human counsellors: A mixed methods study. *International Journal of Mental Health and Addiction*. https://doi.org/10.1007/s11469-025-01595-y
13. Rackoff, G.N., Zhang, Z.Z., Newman, M.G. (2025). Chatbot-delivered mental health support: Attitudes and utilization in a sample of U.S. college students. *Digital Health*. https://doi.org/10.1177/20552076241313401
14. Shvetcov, A., Funke Kupper, J., Zheng, W.-Y., et al. (2024). Passive sensing data predicts stress in university students: A supervised machine learning method for digital phenotyping. *Frontiers in Psychiatry*. https://doi.org/10.3389/fpsyt.2024.1422027
15. Soneson, E., Fazel, M., Goli, P.S., White, S.R. (2025). Are adolescents sensitive about sensitive data? Exploring student concerns about privacy, confidentiality, and data use in health research. *Journal of Adolescent Health*. https://doi.org/10.1016/j.jadohealth.2025.03.004
16. Zhang, Z., Lu, X., Zhang, Y., et al. (2026). Privacy assurances and professional-boundary warnings in generative AI mental health chatbots: A randomized vignette experiment on calibrated trust, overreliance risk, and professional help-seeking intentions. *Frontiers in Psychology*.
17. Zhao, T., Zhao, X., Cheah, K.S.L., Zhang, Y. (2025). ChatGPT, loneliness, and well-being among international PhD students in Malaysia: A mixed-methods study. *International Journal of Mental Health Promotion*.
18. Zivin, K., Eisenberg, D., Gollust, S.E., Golberstein, E. (2009). Persistence of mental health problems and needs in a college student population. *Journal of Affective Disorders*.
19. Kessler, R.C., et al. (2005). Lifetime prevalence and age-of-onset distributions of DSM-IV disorders in the National Comorbidity Survey Replication. *Archives of General Psychiatry*.
