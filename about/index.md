---
layout: page
title: About
permalink: /about/
---

## The founding

The Lanka Software Foundation was conceived by <a href="/about/members#sanjiva">Sanjiva</a> and <a href="/about/members#jivaka">Jivaka</a> in 2001/2. After 16 years in the US, Sanjiva returned to Sri Lanka in 2001. As a long time open source contributor, Sanjiva understood that open source distribution of software was a powerful way to reach the global market. At that time, while everyone was talking about using free and open source software in Sri Lanka, no one was promoting, guiding and supporting the creation of open source software from our side of the world. 

In the early 2000s, Sanjiva was deeply involved in creating the Web services platform (the "WS-*" platform) as part of his work in IBM Research. The Web services platform was about converting the Web and its core standards (HTTP, XML (now JSON), HTML etc.) from an information dissemination system to a distributed computing system. It was also the time that free and open source software was becoming the de facto enabler and accelerator of modern infrastructure, starting with the Linux Operating System, the Apache Web Server, the MySQL Database, the PHP Language (the "LAMP" stack) and many others.

Yet, at the time, contributions to almost every open source project was only by people based in the US and a few western nations. They saw this as an opportunity to create a brand for Sri Lanka's software developers not as a low-cost destination, but rather as a place where smart, creative, hardworking engineers create the software that powers the world.

LSF set out to create an environment to make it possible for Sri Lankan developers to contribute to, and lead, the next generation of platform infrastructure software.


### Members

LSF is registered as a company limited by guarantee in 2003, which is the vehicle for creating not-for-profit busineses in the country. The members serve as the guarantors of the company in terms of financial operation and commitment to purpose.

The members are / were:

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


## Phase 1 (2003 to 2013): Building open source technology around web services & Sahana
This phase is what led to the creation of WSO2 on top of the Apache Axis2 project which LSF developed with a $100K grant from the Swedish International Development Agency (from 2004 to 2005). After WSO2 launched in 2005, LSF continued to do various projects in web services but work in that area slowed down a lot as Sahana took primary focus.


In 2004, after the tsunami we also started the Sahana disaster management platform project which became our focus for many years, eventually culminating in it being donated to a dedicated foundation (the Sahana Software Foundation [1]) in 2009. 

## Phase 2 (2013 to 2018): Open source incubator - building open source businesses

In this phase we attempted to support open source projects in Sri Lanka to become successful global businesses. Unfortunately, I cannot point to any meaningful success in that era.

## Phase 3 (2019-2024): Code for Sri Lanka - building government solutions

In this phase we focused on helping the government of Sri Lanka with various software solutions. While we had some good success (in particular for elections and education), the efforts have not resulted in any permanent impact on Sri Lanka’s digital government platform or architecture. See [2] and [3] for more information.

During this phase, we also collaborated with Prof. Louiqa Raschid from the University of Maryland, a former director of LSF and a long time technical collaborator for me personally, on Karsha, a project aimed at making financial data more structured, accessible, analyzable and available. We still have some budget left over from that work and it will be reserved for future collaboration with Prof. Raschid as she funded much of that work personally. See [4] for more information.



