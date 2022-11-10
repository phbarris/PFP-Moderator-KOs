# Mod Collector Knowledge Object Read Me
This Knowledge Object collection packages moderator functions original developed for the Precision Feedback Pipeline.  

## What is a causal pathway?
A causal pathway represents the relationships among variables and outcomes of interest in a given context. In implementation research, causal pathways specify the structural relationships (mechanism) between implementation strategies and implementation outcomes. Causal pathways account for an initial implementation strategy, moderators, and preconditions that influence the outcome of interest.

*Should causal pathways/moderators/preconditions be described in the context of implementation science? If the intent is to share these moderators and other pipeline components for other people building software for implementation mechanisms, the this would make sense. Are there other use cases for the moderators?*

## What is an implementation strategy?
An implementation strategy is a chosen set of behaviors, tasks, or interventions perceived to address barriers to behavioral and/or organizational change.

## What is a precondition?
A precondition is a factor that is necessary in order for a causal pathway to be activated.

## What is a moderator?
Moderators are functions that given an input, indicates the magnitude of influence of some characteristic on an intervention.

In the case of implementation strategies, a moderator quantifies the magnitude of influence of a factor on that ability of that implementation strategy to achieve it's desired outcome.  

## Who are these moderators for?
Individuals developing software pipelines based on causal pathway design. Individuals wanting to modify existing computable causal pathways.

*Questions to ask:*
- *Who will be accessing these moderators in the future?*
- *-> Other investigators developing precision audit and feedback programs?*
- *Are there other uses for these?*

## What will people use these moderators for?
The packaged moderators in this knowledge object collection can be plugged into computable causal pathway mechanism, to inform the influence of selected characteristics on the magnitude of influence on the intervention represented by the causal pathway.

*Questions to ask*
- *Can these moderators be used outside the mechanisms represented by causal pathways? Or are these primarily intended for representation by causal pathways?*

## What moderators are packaged?
The following moderators are going to be packaged:
1. Gap size
2. Trend slope
3. Monotonic prediction

These moderators function independently

### Gap size
**Description:**

**Inputs:**
- performance_data_df
- comparison_values

**Outputs:**
- goal_gap_size_df


### Trend Slope
**Description:**

**Inputs:**
- performance_data_df
- comparison_values

**Outputs:**
- slope_final_df

### Monotonic prediction
**Description:**

**Inputs:**
- performance_data_df
- comparison_values

**Outputs:**
- trend_df = "no trend", "non-monotonic", or "monotonic"

*Questions to ask*
- *What exactly are the "comparison_value" inputs, and how can the performance and comparison inputs best be described outside of the context of the PFP?*
- *Clarify the outputs/descriptions of the 3 provided moderators*
