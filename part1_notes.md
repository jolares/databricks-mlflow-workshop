# Part 1 Notes


## ML Lifecycle

### Traditional Software Development Lifecycle vs Machine Learning Life Cycle

| Traditional SDLC                         |  MLLC  |
|------------------------------------------|--------|
| goal: meet functional specs              | goal: optimize a metric (e.g accuracy). Constant experimentation is needed to advance towards goal.  |
| quality depends only on code             | quality depends on input data and tuning parameters  |
| generally one can pick a stack and use a few libs | generally one compares + combines many libraries for developing different models, choosing the one (and the best baseline model) that best solves the particular problem at hand  |
| deployment environments are limited      | diverse deployment environments  |


### ML Lifecycle

Many different tools for each stage in the ML Lifecycle, each may be completely
different tools/libraries.

> (see img in minute 12:18)


    +---> Raw data ---> Data Prep ---> Training --->+
    |                                               |
    +--------<--------------<--------------<--------+


- Data Prep: 
    - Data Tunning
- Training: iterative process
    - Hyper-param Tunning
    - Scale
- Deploy:
    - Reproducibility between models while in development/local vs in production/cloud
      (ensuring hp are the same, models are performing as expected, consistently to how they did in development while training and evaluating)

Additional Issues

- ML Platform is often custom to company's, little can be transfered from org to org in terms of how the process abov


----


## MLflow


- API first approach: one can submit runs, log models, metics, etc.
- models are inspired by "lambda functions" that can be deployed in many environments
- open-source, open interface, and modular so indidivual components of MLflow can work independently, as well as together.
