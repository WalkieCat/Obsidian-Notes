## Question 1: Can risks ever be completely removed? Why or why not?
Risk cannot be completely removed because all activities contains some level of unpredictability and uncertainty. In a real situation, risks cannot be removed entirely but can only be minimized [^1]. While some specific risks can be eliminated, there are still some inherent risks that remains. An example is that safety measures can remove the primary risks, other factors such as human errors or environment change can still generate more risks. Therefore, the existence of risk management is crucial. It is the process of minimizing risks to the lowest possibility rather than completely eliminating risks. 

## Question 2: Which is more dangerous? Physical or digital risks? Explain your choice
While there are no definite "more dangerous" risk, the recent surge shows that digital risks are now more prevalent than ever due to our changing cyber landscape [^2]. Within this context, it can be said that digital risks are more dangerous due to their higher likelihood of occurring. As more companies opt for digital solution, the threat of cybersecurity incidents keep on increasing [^3]. These organizations are becoming more exposed to threats such as ransomware, malware and data breaches. All these threats are evolving and becoming increasingly more difficult to respond to.

However, physical risks - such as theft, destruction of infrastructure or equipment malfunction - can still have severe consequences despite having a less frequent occurrence. In conclusion, the level of danger for a risk depends on both the likelihood and impact. While digital risks are becoming more common, physical risks can, in some cases, cause greater damages. Thus, both of these risks need to be managed carefully.

## Question 3: Why are residual risks important in decision making?
Residual risks are risks that remains after controls and mitigation procedure are in place to address the inherent risks. These risks cannot be fully eliminated, and in turns cause damage if they are unaccounted for. If left unmonitored, as the project progress, it can cause significant damage to the entire project. Understanding the residual risks allow the managers to understand whether to implement more controls to address these risks or to classify the risks as acceptable.

# Scenario
Canberra Online Learning (COL) is a university-managed digital platform used by students, academic staff, and administrators. The platform supports online lectures, assignment submissions, grading, and communication between students and staff.  
  
The system stores sensitive information including student personal data, academic records, and assessment materials. It operates on a cloud-based infrastructure and is accessible remotely via the internet.  
  
Recently, the university has identified several concerns:  
- Increase in phishing emails targeting staff accounts  
- Reports of weak passwords among users  
- Occasional system slowdowns during peak exam periods  
- Growing concern about ransomware attacks affecting universities globally  
  
You have been appointed as part of the cyber security team to assess the risks and recommend appropriate actions.

## Task 1: Identify Information Assets
Identify at least five important assets used in the system:

| Assets | Description | Importance (High/Medium/Low) |
| ------ | ----------- | ---------------------------- |
| Student personal database | Contains information about student name, address and possible bank details | High to students |
| Academic records | Contains information about student grades, transcript and results | High to students, staff and university |
| Credentials database | Contains login details for students and staff | High to entire institution |
| The platform itself | The core system that delivers different services to students and staffs | High to entire institution |
| Assignment details | Information about students assessment items | High to staffs, medium to students |


## Task 2: Identify potential security threats for each assets
| Assets | Threat|
| ------- | ------- |
| Student personal database | Data breach, ransomware, phishing attacks  |
| Academic records | Unauthorized modification, ransomware |
| Credentials database | Ransomware, data breach, brute force attacks |
| Learning platform | DDoS attacks |
| Assignment details | Insider misuse (leaking information), ransomware |

## Task 3: Identify weaknesses that could allow the threat to occur
| Assets | Threats | Vulnerabilities |
| ------- | -------- | --------------- |
| Student personal database | Data breach, ransomware, phishing attacks  | Poor access controls, weak encryption/authentications |
| Academic records | Unauthorized modification, ransomware | Poor access controls, lack of auditing |
| Credentials database | Ransomware, data breach, brute force attacks | Lack of encryption, MFA and weak passwords |
| Learning platform | DDoS attacks | Inadequate resources | 
| Assignment details | Insider misuse (leaking information), ransomware | Lack of file permission, no user controls |

## Task 4: Risk analysis
|**Risk**|**Likelihood (1–5)**|**Impact (1–5)**|**Risk Score**|
|---|---|---|---|
|Phishing attack leading to account compromise|5|4|20|
|Weak passwords leading to unauthorised access|5|4|20|
|Ransomware attack on system|4|5|20|
|System slowdown/crash during exams|4|3|12|
|Data breach of student personal data|3|5|15|

## Task 5: Prioritize risks
- The top 2 risks to prioritize are: Phishing attacks and weak passwords
- These were choosing because they have a high likelihood of occurring

## Task 6: Risk management strategy
|**Risk**|**Strategy**|**Justification**|
|---|---|---|
|Phishing attacks | Mitigation | Implement staff training, email filtering, and awareness programs to reduce likelihood|
|Weak passwords | Mitigation | Enforce strong password policies and multi-factor authentication (MFA) to prevent unauthorized access|

## Task 7: Discussion Questions
### Which risk was most critical and why?
Phishing is the most critical attack because it directly affect the users which have a high likelihood to occur, making it easier for a threat actor to gain access to the system. This can be the first step to more serious attacks occurring such as a ransomware or data breaches.

### What could happen if no actions are taken?
If no actions are taken, attackers will gain unauthorized access to these accounts, which can lead to data breaches, leak of sensitive information or system-wide attacks. This could severely damages the university operations and reputations.

### How does your decision align with the organisation’s risk appetite?
The decision aligns with a low risk appetite, as the university handles sensitive data and cannot tolerate high levels of risk. Therefore, high-risk threats such as phishing and weak passwords must be actively reduced through mitigation strategies.

# Part 3 Quantitative Risk Assessment (ROSI) (20-25 mins)

Over the past 5 years, your organisation has accumulated 10,000 customer records. Your annual revenue is $2,000,000, and repeat customers contribute 10% of revenue. Sales staff carry laptops with sensitive data.  
  
Industry data suggests a 47% chance of laptop loss annually. If data is exposed, you may lose all repeat business.  
  
Fraud risk also exists with probability 0.09 and average loss of $14,000 per $1M revenue.

Key Data:

|Item|Value|
|---|---|
|Annual Revenue|$2,000,000|
|Repeat Business|10% ($200,000)|
|Laptop Loss Probability|0.47|
|Fraud Probability|0.09|
|Fraud Loss|$28,000|

  
Proposed Controls:

|Control|Description|Cost|
|---|---|---|
|Laptop Encryption|CyGuard software|$8,000/year|
|Fraud Detection|Auditing software|$2,200/year|

  
Your Tasks:

|Step|Description|
|---|---|
|Step 1|Calculate SLE, ARO, ALE|
|Step 2|Calculate ALE after control|
|Step 3|Calculate ROSI|
|Step 4|Make recommendation|
|Step 5|Recalculate with 25% residual risk|


The organisation holds 10,000 customer records, generating $2,000,000 annually, with $200,000 from repeat customers. Sales laptops store sensitive data, introducing exposure.

**Risk Assessment:**

- **Laptop Loss:** ARO = 0.47, SLE = $200,000 → ALE = $94,000
- **Fraud:** ARO = 0.09, SLE = $28,000 → ALE = $2,520
- **Total ALE Before Controls:** $96,520

**Proposed Controls:**

1. Laptop encryption (CyGuard) – $8,000/year
2. Automated fraud detection – $2,200/year  
    **Total Annual Cost:** $10,200

**ROSI (0% residual risk):**

- Laptop encryption: 1,075%
- Fraud detection: 14.5%
- Combined: 848%  
    **Net Benefit:** $86,320

**ROSI (25% residual risk):**

- Laptop encryption: 781%
- Fraud detection: −85.9%
- Combined: 609%  
    **Net Benefit:** $62,190

**Conclusion:** Both controls are financially justified. Laptop encryption provides a particularly high return, while fraud detection offers qualitative benefits (compliance, reputational protection), even under partial risk reduction.


### REFERENCE:

[^1]: https://www.sbm.itb.ac.id/2024/02/21/risks-cannot-be-eliminated-but-can-be-minimized/

[^2]: https://ia.acs.org.au/article/2025/australian-industry-battles-with-surging-cyber-risk.html

[^3]: https://www.cyber.gov.au/about-us/view-all-content/reports-and-statistics/annual-cyber-threat-report-2024-2025
