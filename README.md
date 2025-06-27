# Reproducing Results from MINDBIGDATA Leaderboard

Leaderboard: [MINDBIGDATA leaderboard](https://mindbigdata.com/).  
So far, many of the methods listed on the leaderboard fail to demonstrate the same performance when independently tested.  
In most cases, the results are equivalent to random guessing, indicating that the reported scores are **not reproducible**.

---

## A Note on One Reproducible Work

One method does yield **reproducible results**, but only by **rejecting a substantial portion of the dataset**.  
This filtering step creates clearer separation between EEG signals corresponding to digits, which enables high accuracy on the remaining data.

However, this approach has serious limitations:
- If a new EEG signal doesn't meet the filtering criteria, the model can't produce a prediction.
- This makes the method unreliable in practical, real-world scenarios.

---

## Final Thoughts

Despite these issues, the reproducible method offers an **optimistic perspective**:  
**EEG signals may contain usable information about higher cognitive processes** — under the right conditions.

Future work should aim to develop models that generalize well **without discarding large portions of the data**. 

