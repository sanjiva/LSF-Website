---
layout: page
permalink: /about/members/
---

# Members

LSF is registered as a company limited by guarantee, which is the vehicle for creating not-for-profit busineses in the country. The members serve as the guarantors of the company in terms of financial operation and commitment to purpose.

<table>
    {% for member in site.data.members %}
        {% assign person = member[1] %}
        <tr>
            <td width="20%" style="vertical-align: top;">
                <img src="{{ site.baseurl }}/{{ person.image }} " width="100%">
            </td>
            <td>
                <p id="{{ member[0] }}">
                    <b> {{ person.name }} </b><br>
                    {{ person.shortbio | markdownify }}
                    {% if person.moreinfo != nil %}
                        More: 
                        <a href="{{ person.moreinfo }}"> {{ person.moreinfo}} </a>
                    {% endif %}
                </p>                
            </td>
        </tr>
    {% endfor %}
</table>