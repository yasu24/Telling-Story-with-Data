| [Home Page](https://github.com/yasu24/Telling-Story-with-Data) | [Data Visualization Critiques](data-visualization-critiques.md) | [Data Visualization Workshops](data-visualization-workshops.md) | [Final Project Part1](final-project-part1.md) | [Final Project Part2](final-project-part2.md) | [Final Project Part3](final-project-part3.md) |

# Final Project Part 2

# Wireframes/storyboards
> Using your sketches developed last week, further develop your story outline and relevant components visually through the use of wireframing/storyboards. Using your outline as a guide, include high-fidelity, individual draft data visualizations of the critical elements of the story you want to share with your reader. Note: you can build these elements out directly in Shorthand this week if you wish.  Reminder: this template is intended to help, but it doesn't substitute for reading through the full homework assignment!  The assignment page on Canvas includes many important details for completing Part II of the final project. 

## Wireframes

Story:

As the Whitehouse announced, President Biden established the "Gun Violence Prevention Office" in Sep 2023.

This unprecedented move comes after a series of tragic shootings and consistent public outcry for stricter gun control. 

Ever since I moved to the US, I've been exposed to numerous gun-related news stories, including those from Pittsburgh.

Coming from Japan, where guns are far less common, my curiosity about this topic spurred this project.

Given the complexities surrounding American history and culture related to guns, this project will objectively focus on "Gun Violence" rather than debating the merits of gun ownership.

In this project, I would like to find any insight based on crime, regulation, or possibly economic data.

The primary goal of this project is to contribute insights towards reducing gun violence and its victims. As such, the intended audience includes governmental officials and policymakers.

Logic:

As-Is

We have the regulation ranking and its points for each state.

<div class='tableauPlaceholder' id='viz1696431366848' style='position: relative'>
  <noscript>
    <a href='#'>
      <img alt='States Ranked by How Strict Their Gun Laws Are ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ca&#47;Category_16964313443170&#47;Regulation&#47;1_rss.png' style='border: none' />
    </a>
  </noscript>
  <object class='tableauViz'  style='display:none;'>
    <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
    <param name='embed_code_version' value='3' /> 
    <param name='site_root' value='' />
    <param name='name' value='Category_16964313443170&#47;Regulation' />
    <param name='tabs' value='no' />
    <param name='toolbar' value='yes' />
    <param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ca&#47;Category_16964313443170&#47;Regulation&#47;1.png' /> 
    <param name='animate_transition' value='yes' />
    <param name='display_static_image' value='yes' />
    <param name='display_spinner' value='yes' />
    <param name='display_overlay' value='yes' />
    <param name='display_count' value='yes' />
    <param name='language' value='ja-JP' />
    <param name='filter' value='publish=yes' />
  </object>
</div>

<script type='text/javascript'>
  var divElement = document.getElementById('viz1696431366848');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width='100%';
  vizElement.style.height=(divElement.offsetWidth*0.6)+'px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
</script>

<img src="Result.png" width="800"/>

If we make a heatmap based on the result, we can show as is.

<img src="HeatMap_Reg.png" width="800"/>

Combined with "the gun death rate per 100k" data, all regulation data has a negative correlation, which means that if any regulation is added, the number of gun deaths will be reduced, which is a great fact.

<img src="HeatMap_Gun.png" width="800"/>

Though there's a noticeable correlation between Regulation strength and Gun Death Rate, determining causality is more complex. 

Case1. Is the high Gun Death Rate a result of lenient regulations? 
Case2. Are regulations lenient because regions haven't historically perceived a need for tighter control due to lower gun death rates? 

Distinguishing between these two scenarios is crucial.

To-Be

According to the analysis, I would recommend implementing the training program for 41 states, which can lead to the result that around 372 people can be saved per 100k every year. 

Gap

How to implement the regulation? The economic, cultural, or historical difficulties would happen.

According to the Everytown Gun Law Rankings, the laws are categorized into 6 groups. We are going to focus on which category is the most effective in preventing the death rate and also what kind of laws work and don't work.

Categories
- Foundational Law
- Gun Industry and Product Safety
- Guns in Public
- Keeping Guns out of the wrong hands
- Policing and Civil rights
- Sales and Permitting

Initially, data was compared between "each state's laws" and "the gun death rate per 100k" to clarify which category is the most effective in preventing death using guns.

<img src="Coef_Category.png" width="800"/>

As shown above, the most efficient category is "Gun Industry and Product Safety". When a regulation is introduced to a state that doesn't have it, the number of deaths is reduced by 2.02 people per 100,000 people.

On the other hand, the least effective one is "Keeping Guns out of the wrong hands", which has only a 1.07 reduction.

When it comes to each regulation, we can see which regulation has more impact on the gun death rate.

<img src="Coefficiency.png" width="800"/>

And we can highlight the biggest and smallest impact items below.

<img src="Coef_top_bottom3.png" width="800"/>

If we focus on each regulation, The most significant impacted law is "Training Required to Purchase Guns", which has 9.09 people per 100,000 people.
This regulation is implemented in only 9 states, therefore, the remaining 41 states can reduce the number of deaths potentially.
Interestingly, the "No Guns in Bars" regulation has the lowest impact with a rate of 0.46, suggesting that restrictions on guns in bars have a lesser influence on gun-related deaths.

It's important to note that this is merely a binary (yes/no) analysis and a more in-depth examination is necessary. For instance, while the study mentions a "waiting period", we need to consider the exact length of time people must wait after purchasing before actually receiving their guns.

In conclusion, this analysis has identified specific areas of regulation that can significantly reduce gun-related tragedies. While the current study employed a binary approach, future research would benefit from more nuanced methodologies, such as machine learning, to extract deeper insights from the data. 

As I plan to reside in the U.S. for some time, gaining an understanding of this topic has personal significance, and I look forward to delving further into this critical issue.

## Storyboards



# User research 

## Target audience
> Include your approach to identifying representative individuals, and who you hope to reach with your story. 

While the primary target audience is governmental officials and policymakers, public opinion is shaped by the masses. Thus, the general public, especially those concerned with gun regulations, are also considered a significant audience for this project.

## Interview script
> List the goals from your research and the questions you intend to ask. 

The main goal of my research is to contribute insights towards reducing gun violence and its victims. 
The main goal of the interview is to clarify if my explanation is "Understandable", "Informative", and "Enhancement" or not.

| Goal | Questions to Ask |
|------|------------------|
| Understandable | Did you catch what is the main point of the explanation? |
| Informative | Did you get any new insight from the presentation? |
| Enhancement | Were there any parts of the presentation that felt confusing or that could be presented more clearly? |

## Interview findings
> Detail the findings from your interviews.  Do not include PII.  Capture specific insights where possible.

Text here!

| Questions               | Interview 1 (briefly describe) | Interview 2 | Interview 3 |
|-------------------------|--------------------------------|-------------|-------------|
| Did you catch what is the main point of the explanation? | Insightful feedback            |             |             |
| Did you get any new insight from the presentation? |                                |             |             |
| Were there any parts of the presentation that felt confusing or that could be presented more clearly? |                                |             |             |


# Identified changes for Part 3
> Document the changes you plan on implementing next week to address any issues identified.  

Text here!

| Research synthesis                       | Anticipated changes for Part 3                                                  |
|------------------------------------------|---------------------------------------------------------------------------------|
| Findings or observations from interviews | Describe what, if any changes you anticipate making to address the observation. |
|                                          |                                                                                 |
|                                          |                                                                                 |
|                                          |                                                                                 |
| ...add more rows as necessary            |                                                                                 |

> ...include any final thoughts you have here. 

Text here!

# Moodboards / personas
> If you did this optional part, include details here.  Otherwise, remove this section

Text here!
