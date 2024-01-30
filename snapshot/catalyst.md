Author: LPX
Status: Draft

# Maintaining Integrity in Catalyst Incentives 

The integrity of community-funded incentives programs plays a pivotal role in maintaining a fair and transparent trading environment. These programs, aimed at rewarding users based on their trading activity and volume, foster a vibrant, competitive community. 

However, the potential for dishonest behavior, such as volume padding or manipulation, poses a significant threat to this ecosystem. It's our duty to safeguard the platform's integrity and ensure equitable reward distribution among participants. This post delves into the need for a robust tier system based on detailed analysis of trading behaviors, designed to promote healthy trading activities while curtailing manipulative practices.

## Dishonest Behavior and Volume Manipulation Defined

Dishonest behavior or volume manipulation on trading platforms refers to activities aimed at distorting or inflating trading volumes to gain an unfair advantage. Key forms of such behavior include:

1. **Wash Trading**: Simultaneously buying and selling securities to create artificial activity and inflate trading volume.
2. **Churning**: Executing trades repeatedly to generate commissions or artificially inflate trading volume, often resulting in little or no financial gain.
3. **Pattern Gaming**: Trading in patterns that exploit the rules or incentives of the platform without contributing to genuine market activity.
4. **Automation**: Utilizing scripts or bots to execute large amounts of trades for the purpose of inflating trading volume.

These practices not only skew perceived market vitality but also unfairly benefit manipulators at the expense of genuine participants, undermining the fairness and competitive spirit of incentives programs.

## Proposed Metrics for Trading Behavior Analysis

### **Adjusted Trade Frequency Ratio (ATFR)**

**Summary**: Quantifies a user's trading frequency, adjusted to include the duration of each trade, providing a measure that reflects not only the number of trades but also the holding time, offering a nuanced view of trading activity.

**Methodology**: To calculate Modified TFR, we first compute the duration between consecutive trades for each user. The total duration of a user's trades is then divided by the average duration of trades across all users, yielding the Modified TFR. This approach weights each trade by its duration, aiming to capture both the volume and engagement in trading activities more accurately.

**Significance**: Modified TFR is significant in distinguishing between users who trade frequently over short durations and those engaged in longer-term trades. High values might indicate a user who executes many trades in rapid succession, potentially highlighting high-frequency trading strategies or efforts to inflate trading volumes.

Adjusted Trade Frequency Ratio (ATFR): [ \text{ATFR} = \frac{\text{Total Duration of User's Trades}}{\text{Average Duration of Trades across all Users}} ]

![equation_1](https://github.com/EvmosGov/proposals/assets/16395727/9c4ae356-b977-4549-b1b4-cfb71dde0d66)


### **Profitability Index (PI)**

**Summary**: PI measures the average profitability per trade, calculated as the total profit or loss normalized by the trade size, providing insight into the effectiveness of a user's trading strategy in terms of gains or losses.

**Methodology**: PI for each user is computed as the sum of profit or loss (PnL) in USD divided by the total size of trades in USD. This ratio conveys the average return on investment per unit of trade size, offering an average profitability metric.

**Significance**: PI serves as a key indicator of trading strategy success. Values close to zero suggest minimal gains or losses per trade, whereas positive or negative values indicate profitable or unprofitable trading patterns, respectively. PI provides a straightforward assessment of trading efficacy.

Profitability Index (PI): [ \text{PI} = \frac{\text{Total Profit or Loss (PnL) in USD of the User}}{\text{Total Size of Trades in USD}} ]

![equation_2](https://github.com/EvmosGov/proposals/assets/16395727/e2ea31b8-3c4a-4b09-9671-551011f99f51)


### **Repetitiveness Index (RI)**

**Summary**: RI measures the variability in trade intervals for each user, aiming to identify patterns in the timing of trades that could suggest automated or systematic trading behaviors.

**Methodology**: RI is calculated by first determining the intervals between consecutive trades. The standard deviation of these intervals is then divided by the mean interval, producing the RI. A lower RI indicates more consistent, repetitive intervals, while a higher RI suggests greater variability.

**Significance**: RI can reveal patterns in trading behavior, with lower values possibly indicating automated trading systems or strategies favoring regular, systematic trade executions. Understanding RI can help identify users with potentially manipulative or strategic behaviors affecting market dynamics or trading volumes.

Repetitiveness Index (RI): [ \text{RI} = \frac{\text{Standard Deviation of Trade Intervals per User}}{\text{Mean Trade Interval per User}} ]

[equation_3](https://github.com/EvmosGov/proposals/assets/16395727/2df469c0-784c-4878-b5e9-c598646fd7fc)

## The Proposed Tier System

Based on the analysis of our metrics, we propose a tier system to categorize users:

- **Tier 1 (Low Concern)**: Exhibits trading behaviors within the 75th percentile. Suggests alignment with expected market patterns.
- **Tier 2 (Moderate Concern)**: Falls between the 75th and 90th percentiles. Indicates elevated trading frequency or suboptimal profitability.
- **Tier 3 (High Concern)**: Exceeds the 90th percentile. Reflects potentially artificial trading volume through excessive frequency, unprofitable trading, or highly repetitive patterns.

This tier system allows us to scrutinize trading behaviors more closely, flagging activities that may warrant further examination for potential manipulation or volume padding.

### Setting Thresholds

To set meaningful threshold values for each metric and tier, the distributions of these metrics across all users were evaluated. This involves identifying points that significantly deviate from the mean (e.g., using standard deviations as a guide) or determining percentiles that best segment the user base according to the tier definitions.

```
# Correcting the approach: Analyzing 'Modified TFR' and 'LMR' directly from the DataFrame
metrics_mean_std_corrected = assessment_df_mod[['Modified TFR', 'LMR']].agg(['mean', 'std']).T

# Revisiting percentiles for classification into tiers, for 'Modified TFR' and 'LMR'
metrics_percentiles_corrected = assessment_df_mod[['Modified TFR', 'LMR']].quantile(q=percentiles/100).T

# Separately handling 'PI' and 'RI' for threshold determination
# For 'PI'
pi_percentiles = user_pi.quantile(q=percentiles/100)

# For 'RI'
ri_percentiles = normalized_ri.quantile(q=percentiles/100)

metrics_mean_std_corrected, metrics_percentiles_corrected, pi_percentiles, ri_percentiles
```

Based on the analysis of our metrics and their distributions, we've determined potential threshold values using percentiles (50th, 75th, 90th, 95th). 

**Adjusted Trade Frequency Ratio (ATFR) Percentiles:**
* Median (50th): 6.258
* 75th Percentile: 44.807
* 90th Percentile: 110.678
* 95th Percentile: 131.837

**Profitability Index (PI) Percentiles:**

* Median (50th): -0.000029
* 75th Percentile: 0.001301
* 90th Percentile: 0.005138
* 95th Percentile: 0.009838

**Repetitiveness Index (RI) Percentiles:**

* Median (50th): 1.073
* 75th Percentile: 1.159
* 90th Percentile: 1.463
* 95th Percentile: 1.595

### Proposed Tier Thresholds:

Tier 1 (Low Concern): Metrics falling within or below the 75th percentile.
- ATFR ≤ 44.807, LMR ≤ 56.964, PI: above -0.000029, RI: within normal range indicating variability in trade intervals.

Tier 2 (Moderate Concern): Metrics falling between the 75th and 90th percentile.
- 44.807 < ATFR ≤ 110.678, 56.964 < LMR ≤ 725.614, PI between -0.000029 and 0.005138 signaling suboptimal trading, RI suggesting some repetitiveness but not excessively low.

Tier 3 (High Concern): Metrics exceeding the 90th percentile, indicating potential concerns.

- ATFR > 110.678, LMR > 725.614, PI ≤ 0.005138 (considering extreme negative values), RI very low, near 1, indicating highly repetitive trading patterns.

## Closing Thoughts

Implementing a comprehensive tier system is a crucial step toward maintaining the integrity of community-funded incentives programs on trading platforms. By leveraging detailed analytics and robust metrics, we can better identify, understand, and address manipulative trading behaviors, ensuring fair and transparent reward distribution. Our goal is to foster a healthy, competitive trading environment where genuine activity is rewarded, and we maintain the integrity of our community pool. 

![Modified_TFR_Distribution](https://github.com/EvmosGov/proposals/assets/16395727/0741f82f-d88d-4f7b-b7ae-014fbbb24d55)
![LMR_Distribution](https://github.com/EvmosGov/proposals/assets/16395727/c6136a0d-612a-4f4c-a8d9-c0b11a537b83)
![PI_Distribution](https://github.com/EvmosGov/proposals/assets/16395727/238ac9b8-403f-46b2-8313-a42ffd0c43ef)
![RI_Distribution](https://github.com/EvmosGov/proposals/assets/16395727/f7ac5d25-76bc-4006-87c2-3e155afdc779)

