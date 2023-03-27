---
layout: post
title:  "Analysis of Violent Crimes"
date:   2023-03-27 10:29:32 +0100
categories: jekyll update
---
Hey

![Bokeh](https://github.com/suneman/socialdata2023/raw/e3c6f2f2d78cd60b4d0514e88f98b945c1af4aca/files/anscombe.png)


<!DOCTYPE html>
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


[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
