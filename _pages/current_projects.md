---
title: Current Projects
permalink: /current_projects/
---
<strong>Bike Comfort Research</strong>
<br>
My final project in my Python class involved taking UDOT road data from the UGRC, and creating a “bike comfort” score based on several factors (speed limit, bike lane type, and road ownership). This final project led to starting a research project to expand the scope of the original tool, with more publicly available data and a better score calculation with machine learning. We are focusing on college towns around Utah, and aim to develop a web tool and app if the analysis beats what is currently available. The paper will be submitted for publication by the end of the semester, and we plan on presenting the results at the UGIC event in Logan in early May. Below is the code from the original tool and a map visualization of the output.
<details>
<summary><b>Bike Comfort Score Code</b></summary>
<br>
<pre>
<code>
            if 1 < speed_limit <= 20:
                comfort_score += 4
            if speed_limit <= 25:
                comfort_score += 3
            if 25 < speed_limit <= 30:
                comfort_score += 2
            if 30 < speed_limit <= 50:
                comfort_score += 1
            if speed_limit > 50:
                comfort_score -= 1
            if speed_limit is None:
                comfort_score += 0

            if bike_right == "2B":
                comfort_score += 1
            if bike_left == "2B":
                comfort_score += 1
            if bike_right == "4B":
                comfort_score += 2
            if bike_left == "4B":
                comfort_score += 2
            if bike_right == "1B":
                comfort_score += 2
            if bike_left == "1B":
                comfort_score += 2
        
            if dot_fclass == "UDOT":
                comfort_score -= 1

</code>
</pre>
</details>
<br>
<img src="https://afielder02.github.io/GISPortfolio/assets/maps/SLC_DEMO.jpg" width="1000" height="1000">
