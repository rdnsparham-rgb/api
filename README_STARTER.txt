Model Project - Starter Files
=============================

Included files:
1. dataset.txt
   - A synthetic Persian conversational dataset (seed) formatted with <|user|> and <|assistant|> tokens.
   - Use as initial training data or augment with your own daily data.

2. index.html
   - A demo UI for chatting with the model (display-only). The heavy model is intended to be run on a GPU server.
   - You can collect user messages locally (localStorage) via the 'افزودن به dataset' button.

3. .github_workflow_train.yml
   - A GitHub Actions workflow template for dispatching a training job.
   - Heavy training must run on self-hosted runners with GPUs or external cloud GPUs.

How to proceed:
- Replace placeholders and write your actual training script (train.py) in the repo.
- Add your heavy compute runner (self-hosted) and use its label when dispatching the workflow.
- Regularly append new data to dataset.txt or collect user-sentences from the demo UI and incorporate them into training.
