---
layout: default
title: Demo
data: [
    ["ag", "ar", "ai"],
    ["be", "bl", "bs"],
    ["fr", "ge", "gl"],
    ["gr", "ju", "lu"],
    ["ne", "nw", "ow"],
    ["sg", "sh", "so"],
    ["sz", "tg", "ti"],
    ["ur", "vd", "vs"],
    ["zg", "zh"]
]

bonus: [
    ["lake_aegeri", "lake_baldegg"],
    ["lake_biel", "lake_brienz"],
    ["lake_constance_main", "lake_constance_west"],
    ["lake_geneva", "lake_hallwil"],
    ["lake_lucerne", "lake_lugano"],
    ["lake_maggiore", "lake_murten"],
    ["lake_neuchatel", "lake_sempach"],
    ["lake_thun", "lake_walen"],
    ["lake_zug", "lake_zurich"],
    ["sihlsee"],
]
---


# Cantons
All 26 Cantons of Switzerland.

<table class="demo-table">
    {% for row in page.data %}
        <tr>
            {% for item in row %}
                <td>
                    <i class="sc-icon-{{ item }}"></i>
                    {% highlight html %}
                    <i class="sc-icon-{{ item }}"></i>
                    {% endhighlight %}
                </td>
            {% endfor %}
        </tr>
    {% endfor %}
</table>

# Bonus: Lakes
The source SVG also contained all major lakes of switzerland. These are also available in the icon font. The naming of the icon could change in the future.

<table class="demo-table">
    {% for row in page.bonus %}
        <tr>
            {% for item in row %}
                <td>
                    <i class="sc-icon-{{ item }}"></i>
                    {% highlight html %}
                    <i class="sc-icon-{{ item }}"></i>
                    {% endhighlight %}
                </td>
            {% endfor %}
        </tr>
    {% endfor %}
</table>