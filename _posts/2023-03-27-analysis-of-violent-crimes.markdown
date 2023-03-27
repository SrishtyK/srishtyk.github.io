---
layout: post
title:  "Analysis of Violent Crimes"
date:   2023-03-27 10:29:32 +0100
categories: jekyll update
---
<!DOCTYPE html>
<html>
<body>
<h1 style="color:darkred;"><i>A STUDY OF CRIMES: ASSAULT, SEX OFFENSES AND PROSTITUTION</i></h1>

<p align="justify">This article presents conclusions drawn from an analysis of assault, prostitution, and forcible sex offenses crime incidents reported in the San Francisco area. Data have been provided thanks to the SF OpenData project and include crime occurrences recorded between 2003 and 2022 (<a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry">2003-2018</a>)
(<a href="https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783">2018-2022</a>).

We present various visualizations concerning the distribution of those crimes over time and the location of the incidents to uncover patterns behind the data. We also cite various articles and reports to help justify what was observed during the analysis.

For clarification, below are the definitions of crimes:

Assault - generally defined as an intentional act that puts another person in reasonable apprehension of imminent harmful or offensive contact. No physical injury is required, but the actor must have intended to cause harmful or offensive contact with the victim and the victim must have thereby been put in immediate apprehension of such contact (<a href="https://www.law.cornell.edu/wex/assault_and_battery">Cornell</a>) 


Prostitution - involves engaging, agreeing, or offering to engage in sexual conduct with another person in return for a fee (<a href="https://www.law.cornell.edu/wex/assault_and_battery">Cornell</a>).

Forcible sex offense - any sexual act directed against another person, without the consent of the victim, including instances where the victim is incapable of giving consent 
(<a href="https://dps.brown.edu/sites/default/files/CLERY%20CRIME%20OFFENSES%20AND%20DEFINITIONS.pdf">Brown</a>)
</p>

<p align="justify">
<img class="crime" src="/assets/images/crime.png" width="500" height="500" style="float: left; clear: left">
This section shows different perspectives on the full dataset, based on hours and weekdays. From the hours perspective we can see that Assault is consistently present through all day, the exception is between 4 and 6 am, where the numbers of Assaults decrease, probably caused by the fact that most people at that hour are asleep or prepare to go to work. Likewise from weekdays we can see that Assault is a crime that has similar numbers through all the week, reaching its peak on Saturday. Moreover Assault among the three crimes has extremely higher numbers respect to the other two. For Prostitution we can notice that most of the activity is taking place during the night on the hours side, on the weekdays it increase during the week, reaching its peak on Thursday, meanwhile during the weekend especially on Sundays it decreases as expected since the weekend it's usually about spending time with the family. For Sex Offences we can also see that is present and consistent through all week, reaching its peak during weekends, on the hours side most of the Sex Offences takes place between 10 pm and 2 am, its peak is at 12 pm.
</p>

<br>

<div >
<img class="heat" src="/assets/images/heat.png" width="500" height="500" style="float: left; clear: left">
<figcaption align="justify"><i>Heat map shows the patterns of assault, prostitution and forcible sex offences changes over the period 2003-2022 in San Francisco. Yearly change can be seen through the heat map. Total number of crimes are grouped into clusters that happened in the period 2003-2022. Zooming in, the global cluster will start breaking up into smaller clusters. Zooming in all the way will result in individual markers.
</i></figcaption>
</div>
<p align="justify">It can be seen through the heat map that the crime rate significantly decreased after 2018 compared to the period 2003-2017, especially in the regions Richmond, Park, Taraval and Ingleside. In Northern and Bayview district, a small change can be seen here as well. But the no change were seen in Central, Tenderloin, and Southern district of San Fancisco.

Historically, Tenderloin has been a crime hub in San Fransico. Huge change were seen in early 19th Century and the neighborhood has always carried a scruffy exterior since then. Years later the Tenderloin boomed during World War II and several million military members passed through the city that helped fill the coffers of the restaurant, bars and nightclubs. Bar girls aka B-girls would hustle men and then were arrested for vagrancy.This eventually led to the prevalance of prostitution in the district.

The Barbary Coast is marred by persistent lawlessness, gambling, administrative graft, and prostitution. Barbary coast grew during the California Gold Rush in late 19th century, where the population grew exponentially and vigilante communities were formed. Since then, it became the hub of crimes.

Significant decrease in assaults were seen after 2018 because SFPD expanded its foot patrol strategy to focus on crime deterrence and quicker response times as well as more engagement with the community.
</p>


<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Bokeh Plot</title>
<style>
      html, body {
        box-sizing: border-box;
        height: 100%;
        margin: 0;
        padding: 0;
      }
    </style>
    <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-3.0.3.min.js"></script>
    <script type="text/javascript">
        Bokeh.set_log_level("info");
    </script>
  </head>
  <body>
    <div id="702f8ff2-e1ad-4c34-9ef3-0ccf11326ad7" data-root-id="p1004" style="display: contents;"></div>
  
    <script type="application/json" id="p1379">
      {"d8f72e37-7dfd-45cf-b565-eabe41be9beb":{"version":"3.0.3","title":"Bokeh Application","defs":[],"roots":[{"type":"object","name":"Figure","id":"p1004","attributes":{"height":500,"max_width":1000,"sizing_mode":"stretch_width","x_range":{"type":"object","name":"FactorRange","id":"p1014","attributes":{"factors":["2003","2004","2005","2006","2007","2008","2009","2010","2011","2012","2013","2014","2015","2016","2017","2018","2019","2020","2021","2022"]}},"y_range":{"type":"object","name":"DataRange1d","id":"p1006","attributes":{"start":0}},"x_scale":{"type":"object","name":"CategoricalScale","id":"p1018"},"y_scale":{"type":"object","name":"LinearScale","id":"p1020"},"title":{"type":"object","name":"Title","id":"p1007","attributes":{"text":"Distribution of crime incidents throughout the years"}},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1056","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1001","attributes":{"selected":{"type":"object","name":"Selection","id":"p1002","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1003"},"data":{"type":"map","entries":[["Year",{"type":"ndarray","array":["2003","2004","2005","2006","2007","2008","2009","2010","2011","2012","2013","2014","2015","2016","2017","2018","2019","2020","2021","2022"],"shape":[20],"dtype":"object","order":"little"}],["ASSAULT",{"type":"ndarray","array":{"type":"bytes","data":"UA9aPJrurD/s8tZXT9CrP3s83KXev6k/webn9ZxVqz+TcMtAKqSrP29ScqH7Daw/qm51GP4Vqz/KD0zctQerP7onsWJE2qo/qj8W6dKsqj8xlvwTwVyrP9e1Mp5FXqo/mi8C1IIfrD/dxribiketP1qWfIEJc60/n3vITJ+spT+7JVQvFSylP7gEM3/Fq6A/NpBzIvF7oj+MIhrsID+kPw=="},"shape":[20],"dtype":"float64","order":"little"}],["PROSTITUTION",{"type":"ndarray","array":{"type":"bytes","data":"Tc4w9f7WvD/pYYisZmi2P4EH9Mn6MrA/EmO9iNDRsj90QUJTxIO7PzovFvvQvrg/wY6uMnKxtT8wM+VznBKzP9lQkTDdDLA/Ho1JcnowpD8ejUlyejCkPwnyQM+QvZo/RJkRrRwJlj93nfgXr+iiP33dqr7JJZ8/tARaLZlIkj88xLqAaUWRP2TCgKwjim0/q5Pdc1k0aj+RsaEiYbpZPw=="},"shape":[20],"dtype":"float64","order":"little"}],["SEX OFFENSES, FORCIBLE",{"type":"ndarray","array":{"type":"bytes","data":"7IkqBOZyqD+hXRZMdhemP19gT1QhMKc/sVDgvm0Jpj/ex/+9ZaCnP3iCZoczlqo/eIJmhzOWqj8w8sEJeVCuP79MPOa0sq4/vHabyjjGsD8tHCHu/GOwP+e8G525PbM/tbIeGFxItD80Gs+BoLi0P/Ub31Od+7c/re6hZX/Klz9xhLjzj0GWP/nghDwoT5I/QOWLfHBCjj+9G525PZOPPw=="},"shape":[20],"dtype":"float64","order":"little"}]]}}},"view":{"type":"object","name":"CDSView","id":"p1057","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1058"}}},"glyph":{"type":"object","name":"VBar","id":"p1053","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"ASSAULT"},"fill_color":{"type":"value","value":"firebrick"},"hatch_color":{"type":"value","value":"firebrick"}}},"nonselection_glyph":{"type":"object","name":"VBar","id":"p1054","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"ASSAULT"},"line_alpha":{"type":"value","value":0.1},"fill_color":{"type":"value","value":"firebrick"},"fill_alpha":{"type":"value","value":0.1},"hatch_color":{"type":"value","value":"firebrick"},"hatch_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"VBar","id":"p1055","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"ASSAULT"},"line_alpha":{"type":"value","value":0.5},"fill_color":{"type":"value","value":"firebrick"},"fill_alpha":{"type":"value","value":0.5},"hatch_color":{"type":"value","value":"firebrick"},"hatch_alpha":{"type":"value","value":0.5}}},"muted":true}},{"type":"object","name":"GlyphRenderer","id":"p1080","attributes":{"data_source":{"id":"p1001"},"view":{"type":"object","name":"CDSView","id":"p1081","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1082"}}},"glyph":{"type":"object","name":"VBar","id":"p1077","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"PROSTITUTION"},"fill_color":{"type":"value","value":"forestgreen"},"hatch_color":{"type":"value","value":"forestgreen"}}},"nonselection_glyph":{"type":"object","name":"VBar","id":"p1078","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"PROSTITUTION"},"line_alpha":{"type":"value","value":0.1},"fill_color":{"type":"value","value":"forestgreen"},"fill_alpha":{"type":"value","value":0.1},"hatch_color":{"type":"value","value":"forestgreen"},"hatch_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"VBar","id":"p1079","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"PROSTITUTION"},"line_alpha":{"type":"value","value":0.5},"fill_color":{"type":"value","value":"forestgreen"},"fill_alpha":{"type":"value","value":0.5},"hatch_color":{"type":"value","value":"forestgreen"},"hatch_alpha":{"type":"value","value":0.5}}},"muted":true}},{"type":"object","name":"GlyphRenderer","id":"p1106","attributes":{"data_source":{"id":"p1001"},"view":{"type":"object","name":"CDSView","id":"p1107","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1108"}}},"glyph":{"type":"object","name":"VBar","id":"p1103","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"SEX OFFENSES, FORCIBLE"},"fill_color":{"type":"value","value":"royalblue"},"hatch_color":{"type":"value","value":"royalblue"}}},"nonselection_glyph":{"type":"object","name":"VBar","id":"p1104","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"SEX OFFENSES, FORCIBLE"},"line_alpha":{"type":"value","value":0.1},"fill_color":{"type":"value","value":"royalblue"},"fill_alpha":{"type":"value","value":0.1},"hatch_color":{"type":"value","value":"royalblue"},"hatch_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"VBar","id":"p1105","attributes":{"x":{"type":"field","field":"Year"},"width":{"type":"value","value":0.9},"top":{"type":"field","field":"SEX OFFENSES, FORCIBLE"},"line_alpha":{"type":"value","value":0.5},"fill_color":{"type":"value","value":"royalblue"},"fill_alpha":{"type":"value","value":0.5},"hatch_color":{"type":"value","value":"royalblue"},"hatch_alpha":{"type":"value","value":0.5}}},"muted":true}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1011","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1035"},{"type":"object","name":"WheelZoomTool","id":"p1036"},{"type":"object","name":"BoxZoomTool","id":"p1037","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1038","attributes":{"syncable":false,"level":"overlay","visible":false,"left_units":"canvas","right_units":"canvas","bottom_units":"canvas","top_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1039"},{"type":"object","name":"ResetTool","id":"p1040"},{"type":"object","name":"HelpTool","id":"p1041"}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1028","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1029","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1030"},"axis_label":"Count","major_label_policy":{"type":"object","name":"AllLabels","id":"p1031"}}}],"below":[{"type":"object","name":"CategoricalAxis","id":"p1022","attributes":{"ticker":{"type":"object","name":"CategoricalTicker","id":"p1023"},"formatter":{"type":"object","name":"CategoricalTickFormatter","id":"p1024"},"axis_label":"Year","major_label_policy":{"type":"object","name":"AllLabels","id":"p1025"}}}],"center":[{"type":"object","name":"Grid","id":"p1027","attributes":{"axis":{"id":"p1022"},"grid_line_color":null}},{"type":"object","name":"Grid","id":"p1034","attributes":{"dimension":1,"axis":{"id":"p1028"}}},{"type":"object","name":"Legend","id":"p1072","attributes":{"click_policy":"hide","items":[{"type":"object","name":"LegendItem","id":"p1073","attributes":{"label":{"type":"value","value":"ASSAULT"},"renderers":[{"id":"p1056"}]}},{"type":"object","name":"LegendItem","id":"p1099","attributes":{"label":{"type":"value","value":"PROSTITUTION"},"renderers":[{"id":"p1080"}]}},{"type":"object","name":"LegendItem","id":"p1128","attributes":{"label":{"type":"value","value":"SEX OFFENSES, FORCIBLE"},"renderers":[{"id":"p1106"}]}}]}}]}}]}}
    </script>
    <script type="text/javascript">
      (function() {
        const fn = function() {
          Bokeh.safely(function() {
            (function(root) {
              function embed_document(root) {
              const docs_json = document.getElementById('p1379').textContent;
              const render_items = [{"docid":"d8f72e37-7dfd-45cf-b565-eabe41be9beb","roots":{"p1004":"702f8ff2-e1ad-4c34-9ef3-0ccf11326ad7"},"root_ids":["p1004"]}];
              root.Bokeh.embed.embed_items(docs_json, render_items);
              }
              if (root.Bokeh !== undefined) {
                embed_document(root);
              } else {
                let attempts = 0;
                const timer = setInterval(function(root) {
                  if (root.Bokeh !== undefined) {
                    clearInterval(timer);
                    embed_document(root);
                  } else {
                    attempts++;
                    if (attempts > 100) {
                      clearInterval(timer);
                      console.log("Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing");
                    }
                  }
                }, 10, root)
              }
            })(window);
          });
        };
        if (document.readyState != "loading") fn();
        else document.addEventListener("DOMContentLoaded", fn);
      })();
    </script>
  </body>
</html>

<p align="justify">
<figcaption align="justify"><i>Interactive figure showing distribution of assault, prostitution and forcible sex offences throught the 2003-2022 period; Each crime is represented by a different color; Yearly crime counts have been divided by the total number of crimes so that for each type of crime bars sum up to 1.
</i></figcaption></p>
<p align="justify">
The above figure clearly shows that the most recent crime rates for all three types of crimes have dropped quite significantly compared to the first decade of the 21st century. We will look into the patterns more deeply and provide possible explanations for them.
</p>
<p align="justify">
Starting in 2003 prostitution crime rate was at a pretty high level. It dropped in the next 2 years only to come back to the previous level in 2007. From that point number of incidents gradually kept getting smaller. The general decreasing tendency in the first decade of the 21st century might have been caused by First Offender Prostitution Program (the so-called "john school") initiative launched in San Francisco in 1995. The program was aimed at educating men arrested for soliciting prostitutes. According to research done by Abt Associates Inc. (FOPP): "The program is effective in producing positive shifts in attitudes and gains in knowledge. More importantly, the program was found to have reduced recidivism."

In the second half of the period, two noteworthy drops can be observed, one around 2012 and the other in 2020. The first of them might have been caused by the passing of Proposition 35 by the Californian government in November 2012 (Prop 35). The proposal made several changes to the state law regarding human trafficking and sex offenses. Most importantly it expanded the definition of human trafficking, increased penalties imposed for human trafficking, and forced registered sex offenders (incl. sex workers) to provide police with personal identifiers for internet communication and activity. All those taken measures could effectively scare away people from involving in those activities. The latter, on the other hand, is almost surely the outcome of covid-19 pandemic. In the period of lockdown and minimal social contact using prostitution services became difficult if not even impossible.
</p>
<p align="justify">
Both of those crimes are classified as violent crimes and share a similar pattern so we will discuss them together.

The distribution of assault incidents is rather steady and even up to 2017. In 2018, however, the crime rate dropped and settled on a new lower level, even decreasing even further briefly in 2020.

Forcible sex offenses, on the other hand, were also steady until 2007 but then started gradually increasing reaching a peak in 2017. In 2018, similarly as in the case of assault, a significant drop is observed but this time its relative magnitude is much greater. Again from 2018, the low crime level was maintained and slightly decreased even more.

Those two cases clearly show a meaningful drop in 2018. So what happened then? According to a CBS article (CBS) based on the SFPD crime reports (Crime reports), there were several initiatives introduced by the police department to minimize those crime rates. Police collaborated closely with community-based anti-violence partners and established Crime Gun Investigations Center. This led to an increase in the number of weapons seized by 25% compared to 2017 and resulted in a decrease in gun-related violence. Moreover, police changed the strategy of patrolling increasing its presence on the streets and shortening the response time. In 2018 UC Berkeley conducted a study showing that the latter had a positive impact on crime deterrence (UC Berkeley study) “The study suggests that a greater visible police presence helped reduce certain crimes in San Francisco in the two months following redeployment,” said Evan White, the head of UC Berkeley-based California Policy Lab. Those initiatives successfully decreased the number of incidents of violent crimes like assaults or forcible sex offenses.
</p>
<p align="justify">
The analysis shows that each of the crimes has a different temporal pattern and magnitude. Assault, having by far the biggest number of incidents, is distributed evenly through the week and the day with an exception of 4-6 AM. Sex offenses, the least common of the crimes, is also even throughout the week but is more common during night hours. Prostitution incidents, on the other hand, are mostly recorded in the middle of the week and are the most highly polarized between day and night time.

Although the crimes differ in those aspects they all decreased in the 2003-2022 period very significantly. Crime rates in the past 4 years are much lower than in the first decade of the 21st century. All drops were impacted by the covid-19 pandemic but there were also different factors like Proposition 35 in case of prostitution or increased patrols and anti-violence initiatives in case of assault and sex offenses. It seems that San Francisco is becoming safer every year.
</p>

</body>
</html>
