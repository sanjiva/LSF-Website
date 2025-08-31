---
layout: page
title: Team
permalink: /about/team/
---
# Our team
<table>
    {% for person in site.team %}
        <tr>
            <td width="20%" style="vertical-align: top;">
                <img src="{{ site.baseurl }}/{{ person.image }} " width="100%">
            </td>
            <td>
                <p>
                    Name: <b>{{ person.title }}</b><br>
                    Role: <b>{{ person.position }}</b><br>
                    Start Date: <b>{{ person.start_date }}</b><br>
                    Projects:
                        <b>{% for p in person.projects %}
                            <a href="{{ site.baseurl }}/projects/{{ p }}">{{ p }}</a>
                        {% endfor %}</b>
                    {{ person.content | markdownify }}
                </p>
                <p>
                    <a href="{{ person.linkedin }}">
                        <img src="{{ site.baseurl }}/assets/images/linkedin.png" width="5%"/>
                    </a>
                </p>                
            </td>
        </tr>
    {% endfor %}
</table>
