# Digital Feedback Intervention Moderator (D-FIM) Knowledge Object

This knowledge object (KO) contains a collection of moderator functions **specific to digital feedback interventions**. 

## What is a moderator?

Moderators are functions that, given an input, calculate the magnitude of influence of the input's characteristics on an intervention. Moderators are frequently discussed in the context of implementation strategies and causal pathways. 

A **causal pathway** represents the relationships among variables and outcomes of interest in a given context. In implementation research, causal pathways specify the structural relationships (a mechanism) between implementation strategies and their outcomes. When applied to implementation strategies, causal pathways attempt to describe the implementation strategy using inputs, moderators, and preconditions that influence the outcome of the strategy.

An **implementation strategy** is a chosen set of behaviors, tasks, or interventions perceived to address barriers and facilitators to behavioral or organizational change. 

A **precondition** is a factor that is necessary for a causal pathway to be activated.

## What is in the D-FIM KO?

The D-FIM KO contains a collection of moderators specific to causal pathways of digital feedback interventions, as identified by feedback theory. The packaged moderators in D-FIM can be plugged into computable casual pathway mechanisms to inform the magnitude of the influence of selected characteristics on the feedback intervention represented by the causal pathway.

### Included Moderators:
- Gap size: *Assess the magnitude of influence of the gap between inputs*
- Trend slope: *Assess the magnitude of influence of the slope trend of inputs*
- Monotonicity prediction: *Assess the magnitude of influence of monotonic & non-monotonic trends of the inputs.

### Moderator inputs

All moderators in the D-FIM KO function independently of each other. D-FIM requires two inputs:
1. Performance data - a data frame containing measure names, the number of times the measure was passed, the number of times the measure was flagged, and the total number of times the measure was observed.
2. Comparison values - a *data frame(?)* containing the measure names, comparison values, and comparison type.

### Moderator outputs

The D-FIM KO outputs results from all the included moderators into a single data frame. The output data frame (mod_df) contains the measure name, performance data, comparison type, gap size, trend slope, and monotonicity prediction.
