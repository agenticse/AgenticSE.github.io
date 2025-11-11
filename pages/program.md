---
layout: page
title: Program & Accepted Papers (AgenticSE’25)
description: Unified schedule with times, sessions, paper titles, and authors; plus the complete list of accepted papers.
schedule:
  - t: "8:45–9:00"
    session: "Opening"
    type: "opening"
    title: "Welcome and introduction"

  - t: "9:00–10:00"
    session: "Session 1"
    type: "keynote"
    title: "Building Jules, Google's first external coding agent"
    authors_text: "Alexander Mossin; Mehadi Hassen (Google)"

  - t: "10:00–10:30"
    session: ""
    type: "break"
    title: "Coffee Break"

  - t: "10:30–10:55"
    session: "Session 2"
    type: "paper"
    pid: 55
  - t: "10:55–11:20"
    session: "Session 2"
    type: "paper"
    pid: 61
  - t: "11:20–11:35"
    session: "Session 2"
    type: "paper"
    pid: 76
  - t: "11:35–11:50"
    session: "Session 2"
    type: "paper"
    pid: 54
  - t: "11:50–12:00"
    session: "Session 2"
    type: "buffer"
    title: "Buffer"

  - t: "12:00–14:00"
    session: ""
    type: "break"
    title: "Lunch Break"

  - t: "14:00–15:00"
    session: "Session 3"
    type: "keynote"
    title: "Trae Agent: SOTA Open-source AI Coding Agent for SWE-bench"
    authors_text: "Chao Peng (ByteDance)"
  - t: "15:00–15:25"
    session: "Session 3"
    type: "paper"
    pid: 70
  - t: "15:25–15:30"
    session: "Session 3"
    type: "buffer"
    title: "Buffer"

  - t: "15:30–16:00"
    session: ""
    type: "break"
    title: "Coffee Break"

  - t: "16:00–16:15"
    session: "Session 4"
    type: "paper"
    pid: 99
  - t: "16:15–16:30"
    session: "Session 4"
    type: "paper"
    pid: 41
  - t: "16:30–16:55"
    session: "Session 4"
    type: "paper"
    pid: 90
  - t: "16:55–17:00"
    session: "Session 4"
    type: "buffer"
    title: "Buffer"

  - t: "17:00–17:15"
    session: "Closing"
    type: "closing"
    title: "Wrap-up, acknowledgments, and discussion"
---

<style>
  .responsive-table { width: 100%; overflow-x: auto; -webkit-overflow-scrolling: touch; }
  .responsive-table table { width: 100%; border-collapse: collapse; }
  .responsive-table th, .responsive-table td { padding: 8px; border-bottom: 1px solid #ddd; text-align: left; }
  .responsive-table thead { background: #f7f7f7; }
  .muted { color: #666; font-style: italic; }
  .pill { display: inline-block; padding: 2px 8px; border-radius: 12px; background: #eef; font-size: 12px; margin-left: 6px; }
  @media (max-width: 700px) {
    .responsive-table th, .responsive-table td { padding: 6px; }
  }
  .paper-list h4 { margin-bottom: 4px; }
  .paper-list p { margin-top: 0; margin-bottom: 14px; }
  .session-badge { font-size: 12px; color: #555; }
  .program-note { margin-top: 0; color: #555; }
  .section-divider { margin: 28px 0; border-top: 1px solid #e5e5e5; }
  .keynote { font-weight: bold; }
  .break { color: #555; }
  .buffer { color: #777; font-style: italic; }
  .opening, .closing { font-weight: bold; }
  .pid { color: #666; font-size: 12px; margin-left: 6px; }
  .type { color: #555; font-size: 12px; margin-left: 6px; }
  .author-affil { color: #666; }
</style>

### Program

{% assign apapers = site.data.accepted_papers_2025 %}

<div class="responsive-table">
  <table>
    <thead>
      <tr>
        <th style="width: 120px;">Time</th>
        <th style="width: 110px;">Session</th>
        <th>Title</th>
        <th>Authors</th>
      </tr>
    </thead>
    <tbody>
    {% for item in page.schedule %}
      {% assign row_class = item.type %}
      <tr class="{{ row_class }}">
        <td><strong>{{ item.t }}</strong></td>
        <td>{% if item.session %}{{ item.session }}{% endif %}</td>
        <td>
          {% if item.type == 'paper' and item.pid %}
            {% assign paper = apapers | where: 'pid', item.pid | first %}
            {% if paper %}
              <strong>{{ paper.title }}</strong>
              <span class="type">({{ paper.type_submission | downcase }})</span>
            {% else %}
              <strong>Paper #{{ item.pid }}</strong>
            {% endif %}
          {% else %}
            {% if item.type == 'keynote' %}
              <span class="keynote">Keynote:</span> <strong>{{ item.title }}</strong>
            {% else %}
              <span class="{{ item.type }}">{{ item.title }}</span>
            {% endif %}
          {% endif %}
        </td>
        <td>
          {% if item.type == 'paper' and item.pid %}
            {% assign paper = apapers | where: 'pid', item.pid | first %}
            {% if paper and paper.authors %}
              {% capture author_names %}{% endcapture %}
              {% for a in paper.authors %}
                {% assign full = a.first | append: ' ' | append: a.last %}
                {% if forloop.first %}
                  {% capture author_names %}{{ full }}{% endcapture %}
                {% else %}
                  {% capture author_names %}{{ author_names }}, {{ full }}{% endcapture %}
                {% endif %}
              {% endfor %}
              {{ author_names }}
            {% endif %}
          {% elsif item.type == 'keynote' %}
            {% if item.authors_text %}{{ item.authors_text }}{% endif %}
          {% else %}
            &nbsp;
          {% endif %}
        </td>
      </tr>
    {% endfor %}
    </tbody>
  </table>
  <div class="session-badge muted">Note: Session numbers are for flow grouping; buffers allow transitions.</div>
  <div class="muted">Durations (guideline): Long papers 25 min incl. Q&amp;A; Short &amp; Talk-only 15 min incl. Q&amp;A; Keynotes 60 min; Opening/Closing 15 min.</div>
  <div class="muted">Workshop date: November 20, 2025 (co-located with ASE’25).</div>
  <div class="section-divider"></div>
</div>

### Accepted Papers

{% assign by_type = apapers | group_by: 'type_submission' | reverse %}
{% for grp in by_type %}

#### {{ grp.name }}

<div class="paper-list">
{% assign sorted = grp.items | sort: 'pid' %}
{% for p in sorted %}
  <h4>{{ p.title }}</h4>
  {% if p.authors %}
    {% capture a_list %}{% endcapture %}
    {% for a in p.authors %}
      {% assign full = a.first | append: ' ' | append: a.last %}
      {% if forloop.first %}
        {% capture a_list %}{{ full }}{% endcapture %}
      {% else %}
        {% capture a_list %}{{ a_list }}, {{ full }}{% endcapture %}
      {% endif %}
    {% endfor %}
    <p class="author-affil">{{ a_list }}</p>
  {% endif %}
{% endfor %}
</div>
<div class="section-divider"></div>
{% endfor %}
