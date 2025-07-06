# Mental-Workload-Estimation-Using-N-Back-Task

## Aim:

Conducting EEG analysis to identify neural signatures across cognitive load levels, from low-demand to high-intensity tasks.

## Working memory task details:

The task consisted of total Nine blocks with 3 blocks of each 1back,2back and 3back 
After each block there was a short 30 second break (lets call it 30s)
And after every 3 blocks there was a 2 min break. (Lets call it 120s)

The exact order was: 
[1back-30s-2back-30s-3back-120s-2back-30s-3back-30s-1back-120s-3back-30s-1back-30s-2back]

The .edf file I shared contains a participants EEG data while performing the task.
The .edf file contains specific annotations for stimuli type (target or non target), stimulus appearance, key presses, start of the break.

These are the specific annotations: 
```
mkr1 = ['100'] # for appearance of target stimuli
mkr2 = ['110'] # for appearance of non-target stimuli
mkr3 = ['200'] # for correct keypress
mkr4 = ['220'] # for incorrect keypress

mkr5 = ['301'] #for start of one-back task
mkr6 = ['302'] #for start of two-back task
mkr7 = ['303'] #for start of three-back task
```
## Tasks:

(Load means: 1 back, 2 back, 3 back)

1. EEG data preprocessing (you can start by the subject data I have provided for pre and post sim)
2. Band power analysis: determine change of band powers b/w breaks and across different loads
3. Go through literature to understand neural correlates of working memory and what ERP markers exist.
4. ERP analysis: within subject for different loads, across subject for each load. 
5. Check how that ERP is changing (across high load vs low load, and between pre vs post stim).


## Progress:

1. Preprocessed data by manually removing bad channels, applying Independent Component Analysis for eye artifact removal.
2. Produced topomaps and average band power plots for delta through gamma bands for comparative frequency-band analysis.
3. Plotted spectrograms for different channels estimating the effect of breaks and different mental workloads on EEG signals.

## Some Snippets from the files
![image](https://github.com/user-attachments/assets/cd92fc1d-ca46-405d-b666-4438242e7dfe)
Colab File - https://colab.research.google.com/drive/1QEtj7pzZCxl3hRHp8uHctWtLIf4EtKIk?usp=sharing
![image](https://github.com/user-attachments/assets/7852138b-5a7c-4889-8a2a-a4632b3fefdd)
Colab File - https://colab.research.google.com/drive/1kqngNlFxB1OBIdsUJ2F4ktW0xHPAHcUB?usp=sharing
![image](https://github.com/user-attachments/assets/a5ca7d46-2171-4b69-abdd-1af8e5a97307)
Colab File - https://colab.research.google.com/drive/1VjnTWCnOlSde0UgU-MywilEKspQ-oNCw?usp=sharing

