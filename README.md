# Lecture on Data Pipelines

### From lecture on 2025-02-27
### Credit to Daniel Chen and DSCI 310 Course

This lecture goes over:

- How to split your data analysis into r scripts
  - Making the files have one main purpose
  - easier to find code you want, and adjust/add features
  - easier to collaborate, people target individual files
  - each person just re-runs work at the end
  
- Make
  - A tool that allows you to save these steps into "targets"
  - give it a special name like report/analysis and the make file will run all those
  - similar to making an .sh file and running all scripts
  - bash analysis.sh
  - no spaces allowed
  - can also put docker command in make file, like docker compose
  - then you run the make folder like:
  
```bash
make <action you want to run>
```

How to run the analysis:

```bash
Rscript 01-load_clean.R
Rscript 02-eda.R
Rscript 03-model.R
Rscript 04-analyze.R
```


```bash
quarto render
```