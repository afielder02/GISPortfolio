---
title: Current Projects
permalink: /current_projects/
---
<strong>Bike Comfort Research<strong>

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

<img src="https://afielder02.github.io/GISPortfolio/assets/maps/SLC_DEMO.jpg" width="1000" height="1000">
