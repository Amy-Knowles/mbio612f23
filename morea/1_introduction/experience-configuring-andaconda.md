---
title: "Configuring Anaconda"
published: true
morea_id: experience-configuring-andaconda
morea_type: experience
morea_summary: "Adding and configuring the R Kernel in Anaconda"
morea_sort_order: 1
morea_labels:
  - video
---

# Configuring Anaconda

Watch the video below to learn how to integrate an R kernel with Anaconda and set it up for use in a Jupyter notebook.

<div style="padding:56.31% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/741048061?h=bf3b987b55&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen style="position:absolute;top:0;left:0;width:100%;height:100%;" title="Week_1_configure_anaconda_with_R_"></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>

### Code to Configure R and Display the version of R installed

```R 
### After Starting the terminal (Click Base (root) and then open Terminal)
### Paste the following into the terminal

conda config --add channels conda-forge    
conda config --set channel_priority strict    
conda search r-base  
conda create -n r-mbio612
conda activate r-mbio612  
conda install -c conda-forge r-base=4.3
conda install jupyter
### !DO NOT PASTE THE CODE BELOW INTO THE TERMINAL!
```

```R
### After Starting The R console (Type R and wait for the ">", called the prompt)
### Paste the following into the terminal

install.packages("IRkernel")
IRkernel::installspec()
```

```R
### Type the following in Jupyter cell to display the R version installed
R.Version()
```

## Submission instructions

No submission is required for this module.



