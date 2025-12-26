## EEG Fractal Dimension Analysis During Resting State and Mathematical Exercises

https://physionet.org/content/eegmat/1.0.0/

In this project, we calculated and analyzed the variation of the fractal dimension in EEG signals recorded from a group of thirty participants during a resting state and while performing mental arithmetic tasks. The central goal was to investigate whether changes in the fractal dimension could reflect cognitive effort and correlate with task performance. More broadly, the exploration of fractal dimension variations in EEG signals could eventually serve as a tool for identifying preclinical markers of neurological or psychiatric conditions.

The EEG dataset used for this study is publicly available at PhysioNet (EEGMat) and contains recordings from thirty subjects both at rest and during the execution of relatively simple mental multiplication problems. The EEG recordings were captured from twenty-one channels, including frontal (Fp1, Fp2, F3, F4, F7, F8), temporal (T3, T4, T5, T6), parietal (P3, P4, Pz), occipital (O1, O2), and central (C3, C4, Cz) locations. The signals were sampled at 500 Hz, bandpass filtered from 0.5 Hz to 45 Hz, and recorded for approximately 182 seconds per session. Each participant has two files: one corresponding to the resting state and one to the arithmetic task.

To obtain a reliable estimate of fractal dimension, each EEG channel was divided into nine segments of 20 seconds. Shorter blocks were used to avoid over-smoothing and better capture temporal variability. For each segment, the Higuchi fractal dimension was calculated using the Antropy library, and the average across segments was taken to obtain a single representative fractal dimension per channel per session. The variation in fractal dimension was calculated as the difference between task and resting state for each channel and subject.

Participants were divided into two groups based on task performance. Those who solved the majority of problems correctly were labeled as “passed” (1), while those who did not were labeled as “failed” (0). The primary statistical analysis consisted of comparing the variation in fractal dimension between these two groups using the Mann–Whitney U test, which is appropriate for two independent groups and does not assume normality of the data.

Results indicated that for all EEG channels, the variation in fractal dimension did not differ significantly between participants who passed and those who failed the task. For example, in the Fp1 channel, the p-value was 0.536, with slightly higher average variation in the passed group, but this difference was not statistically significant. Similar results were observed across all channels, suggesting that, within this dataset and under these conditions, fractal dimension variation does not correlate with arithmetic task performance.

Despite the lack of statistically significant differences, these analyses provide a foundation for future work. Potential directions include increasing the sample size to improve statistical power, using more complex or longer-duration cognitive tasks to amplify cognitive load effects, and performing regional analyses by grouping channels into frontal, temporal, parietal, occipital, and central regions. Other avenues include exploring the temporal dynamics of fractal dimension using sliding windows, investigating clinical applications as early biomarkers of neurological or psychiatric disorders, combining EEG fractal measures with other physiological signals for multimodal analysis, and applying machine learning methods to predict cognitive performance or classify subjects based on fractal dimension patterns.

In summary, this project presents a methodology to calculate and analyze EEG fractal dimension variation across multiple channels and cognitive conditions, providing a framework for both cognitive neuroscience research and potential clinical applications, while also highlighting future areas for study.




