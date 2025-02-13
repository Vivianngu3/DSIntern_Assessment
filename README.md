# StarCraft Player Ranking Conclusion

## 1. Executive Summary
We analyzed player behavior in Starcraft to predict player ranks using performance data. Our best model achieved ~47-50% accuracy, meaning we can predict ranks with moderate confidence. The findings reveal that reaction speed, actions per minute (APM), and hotkey usage are the most important factors for higher ranks.
Why This Matters:
Game Developers: Improve matchmaking by incorporating skill-based performance metrics.
Players: Understand key skills that contribute to ranking up.
Coaches & Analysts: Use data-driven insights to refine training programs.

## 2. Key Insights from the Analysis
#### What Factors Determine Player Rank?
**The model identified the top factors that separate high-ranking from low-ranking players:**
1. Reaction Speed (Action Latency) - Faster responses lead to better performance.
2. Actions Per Minute (APM) - Players who execute more actions per minute tend to achieve higher ranks.
3. Hotkey Usage - Effective hotkey management improves strategic control.
4. Game Experience (Total Hours Played) - More experienced players tend to perform better.
5. Consistency in Play Actions - Maintaining a steady pattern of actions contributes to ranking up.


## Model Performance Summary

| Model Variant | Accuracy | Key Observations |
|:----------: | :----------: | :----------: |
| Logistic Regression | ~41.7% | Struggles with mid-level ranks, better for higher ranks. |
| Random Forest (Default) | ~44.9% | Performs better than Logistic Regression but misses some ranks. |
| Random Forest (Balanced Data) | ~39.8% | Improved recall for underrepresented ranks but lower overall accuracy. |
| Random Forest (Feature Selection) | ~41.2% | Better rank balance, slight accuracy drop. |
| Random Forest (Tuned) | 47-50% | Best-performing model with improved generalization. |


## 3. Key Takeaways for Stakeholders
For Game Developers
Improve matchmaking by incorporating key skill-based metrics into ranking algorithms. Consider rewarding players who demonstrate strong reaction speed and strategic control.
For Players
Prioritize improving APM, reaction time, and hotkey efficiency to climb ranks. Experience matters, but strategic play is more important than total hours played.
Based on these findings, players looking to improve their rank should focus on:
Increasing APM: Train with practice drills to improve the speed of actions.
Exploring the Map More: Make scouting a habit to gain strategic advantages.
Using the Minimap Effectively: Learn to attack and issue commands via the minimap.
Mastering Hotkeys: Assign critical commands to hotkeys for faster execution.
Reducing Action Latency: Practice fluid gameplay to minimize delays between actions.
For Coaches & Analysts
Focus on training techniques that enhance reaction speed and decision-making. Use data-driven performance tracking to monitor player progress.

## 4. Next Steps & Future Improvements
Try Advanced Machine Learning Models (XGBoost, Neural Networks) to enhance accuracy. 
Explore Real-Time In-Game Analysis to provide live coaching insights. 
Use More Player Data (such as in-game decision-making patterns) for better predictions.
By leveraging these insights, we can create a more engaging and balanced competitive gaming environment while helping players improve their skills strategically.

