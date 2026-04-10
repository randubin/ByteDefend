---
layout: page
title: datasets
permalink: /datasets/
description: Open datasets released by ByteDefend Cyber Lab and the Ariel Cyber Innovation Center for cybersecurity research.
nav: true
nav_order: 2
---

<!-- Datasets Page -->
<div class="datasets-page">

  <p style="font-size:.95rem; margin-bottom:2.5rem; color:var(--global-text-color-light);">
    Open datasets released by <strong>ByteDefend Cyber Lab</strong> &amp; the <strong>Ariel Cyber Innovation Center</strong>
    for advancing cybersecurity research. We encourage the community to build on these resources.
  </p>

  <!-- Dataset Card -->
  <div class="dataset-card" style="
    border:1px solid var(--global-divider-color, #e0e0e0);
    border-left: 5px solid #0a66c2;
    border-radius:10px;
    padding:1.8rem 2rem;
    margin-bottom:2rem;
    background:var(--global-bg-color, #fff);
    box-shadow:0 2px 12px rgba(0,0,0,.07);
  ">

    <!-- Header -->
    <div style="display:flex; align-items:flex-start; justify-content:space-between; flex-wrap:wrap; gap:1rem; margin-bottom:1.2rem;">
      <div>
        <div style="display:flex; align-items:center; gap:.7rem; margin-bottom:.4rem;">
          <span style="font-size:1.6rem;">🔑</span>
          <h2 style="margin:0; font-size:1.2rem; font-weight:700; color:var(--global-text-color);">
            API Traffic Research Dataset Framework (ATRDF)
          </h2>
        </div>
        <div style="font-size:.8rem; color:var(--global-text-color-light);">
          <strong>Ariel Cyber Innovation Center &lt;&gt; Cisco Competition</strong> &bull;
          Released 2023 &bull; Shmuel Lavian &amp; Ariel University ACIC
        </div>
      </div>
      <div style="display:flex; gap:.6rem; flex-wrap:wrap;">
        <a href="https://github.com/ArielCyber/Cisco_Ariel_Uni_API_security_challenge"
           target="_blank"
           style="display:inline-flex; align-items:center; gap:.4rem; padding:.45rem 1rem;
                  background:#24292e; color:#fff; border-radius:6px; font-size:.78rem;
                  font-weight:600; text-decoration:none;">
          <i class="fab fa-github"></i> View on GitHub
        </a>
        <a href="https://doi.org/10.1016/j.cose.2024.104249"
           target="_blank"
           style="display:inline-flex; align-items:center; gap:.4rem; padding:.45rem 1rem;
                  background:#0a66c2; color:#fff; border-radius:6px; font-size:.78rem;
                  font-weight:600; text-decoration:none;">
          <i class="fas fa-file-alt"></i> Related Paper
        </a>
      </div>
    </div>

    <!-- Description -->
    <p style="font-size:.88rem; line-height:1.65; margin-bottom:1.3rem; color:var(--global-text-color);">
      A multi-level benchmark dataset of HTTP API traffic for binary and multi-class classification of
      malicious vs. benign API requests. Contains four progressively harder datasets covering diverse
      attack types, endpoint complexities, and parameter structures. Includes training, test, and
      held-out validation splits with a baseline Jupyter notebook.
    </p>

    <!-- Stats row -->
    <div style="display:grid; grid-template-columns:repeat(auto-fit,minmax(130px,1fr)); gap:.8rem; margin-bottom:1.4rem;">
      {% assign stats = "4 Datasets|7 Attack Types|HTTP API Traffic|JSON Format" | split: "|" %}
      {% assign icons = "fas fa-database|fas fa-skull-crossbones|fas fa-network-wired|fas fa-code" | split: "|" %}
      <div style="text-align:center; padding:.8rem; background:rgba(10,102,194,.06); border-radius:8px;">
        <i class="fas fa-database" style="color:#0a66c2; font-size:1.2rem; margin-bottom:.3rem; display:block;"></i>
        <div style="font-weight:700; font-size:.9rem; color:var(--global-text-color);">4 Datasets</div>
        <div style="font-size:.72rem; color:var(--global-text-color-light);">Progressive difficulty</div>
      </div>
      <div style="text-align:center; padding:.8rem; background:rgba(10,102,194,.06); border-radius:8px;">
        <i class="fas fa-skull-crossbones" style="color:#0a66c2; font-size:1.2rem; margin-bottom:.3rem; display:block;"></i>
        <div style="font-weight:700; font-size:.9rem; color:var(--global-text-color);">7 Attack Types</div>
        <div style="font-size:.72rem; color:var(--global-text-color-light);">SQLi, XSS, RCE, Log4J…</div>
      </div>
      <div style="text-align:center; padding:.8rem; background:rgba(10,102,194,.06); border-radius:8px;">
        <i class="fas fa-network-wired" style="color:#0a66c2; font-size:1.2rem; margin-bottom:.3rem; display:block;"></i>
        <div style="font-weight:700; font-size:.9rem; color:var(--global-text-color);">HTTP API Traffic</div>
        <div style="font-size:.72rem; color:var(--global-text-color-light);">Real-world requests</div>
      </div>
      <div style="text-align:center; padding:.8rem; background:rgba(10,102,194,.06); border-radius:8px;">
        <i class="fas fa-code" style="color:#0a66c2; font-size:1.2rem; margin-bottom:.3rem; display:block;"></i>
        <div style="font-weight:700; font-size:.9rem; color:var(--global-text-color);">Baseline Notebook</div>
        <div style="font-size:.72rem; color:var(--global-text-color-light);">Python / scikit-learn</div>
      </div>
    </div>

    <!-- Dataset table -->
    <h4 style="font-size:.9rem; font-weight:700; margin-bottom:.7rem; color:var(--global-text-color);">Datasets Overview</h4>
    <div style="overflow-x:auto;">
    <table style="width:100%; border-collapse:collapse; font-size:.82rem;">
      <thead>
        <tr style="background:rgba(10,102,194,.08); text-align:left;">
          <th style="padding:.55rem .8rem; font-weight:700; color:var(--global-text-color);">Dataset</th>
          <th style="padding:.55rem .8rem; font-weight:700; color:var(--global-text-color);">Description</th>
          <th style="padding:.55rem .8rem; font-weight:700; color:var(--global-text-color);">Task</th>
          <th style="padding:.55rem .8rem; font-weight:700; color:var(--global-text-color);">Baseline F1</th>
        </tr>
      </thead>
      <tbody>
        <tr style="border-bottom:1px solid var(--global-divider-color, #eee);">
          <td style="padding:.5rem .8rem; font-weight:600; color:#0a66c2;">Dataset 1</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">Basic API traffic, fewest attacks &amp; endpoints</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">Binary (Benign / Malicious)</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">0.968</td>
        </tr>
        <tr style="border-bottom:1px solid var(--global-divider-color, #eee); background:rgba(0,0,0,.02);">
          <td style="padding:.5rem .8rem; font-weight:600; color:#0a66c2;">Dataset 2</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">More attacks, ~2× endpoints, higher randomization</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">Binary</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">0.978</td>
        </tr>
        <tr style="border-bottom:1px solid var(--global-divider-color, #eee);">
          <td style="padding:.5rem .8rem; font-weight:600; color:#0a66c2;">Dataset 3</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">Complex parameters, authentic traffic patterns</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">Binary + Attack Type (7 classes)</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">0.940 / 0.940</td>
        </tr>
        <tr>
          <td style="padding:.5rem .8rem; font-weight:600; color:#0a66c2;">Dataset 4</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">Advanced: API redirection, deeper access, more types</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">Binary + Attack Type (7 classes)</td>
          <td style="padding:.5rem .8rem; color:var(--global-text-color);">0.837 / 0.866</td>
        </tr>
      </tbody>
    </table>
    </div>

    <!-- Attack types -->
    <h4 style="font-size:.9rem; font-weight:700; margin:1.3rem 0 .7rem; color:var(--global-text-color);">Attack Types Covered</h4>
    <div style="display:flex; flex-wrap:wrap; gap:.4rem;">
      {% assign attacks = "SQL Injection|Directory Traversal|Remote Code Execution (RCE)|Cookie Injection|Cross-Site Scripting (XSS)|Log4J|Log Forging" | split: "|" %}
      {% for attack in attacks %}
      <span style="font-size:.75rem; font-weight:600; padding:.25rem .7rem;
                   background:rgba(220,38,38,.08); color:#dc2626;
                   border:1px solid rgba(220,38,38,.2); border-radius:20px;">{{ attack }}</span>
      {% endfor %}
    </div>

    <!-- Citation -->
    <h4 style="font-size:.9rem; font-weight:700; margin:1.4rem 0 .6rem; color:var(--global-text-color);">
      <i class="fas fa-quote-left" style="font-size:.8rem; margin-right:.4rem; opacity:.6;"></i>Citation
    </h4>
    <div style="background:var(--global-code-bg-color, #f6f8fa); border-radius:6px; padding:1rem 1.2rem; font-family:monospace; font-size:.74rem; line-height:1.6; color:var(--global-text-color); overflow-x:auto;">
@misc{Lavian_ATRDF_2023,<br>
&nbsp;&nbsp;author = {Lavian, Shmuel and {Ariel University, Ariel Cyber Innovation Center (ACIC)}},<br>
&nbsp;&nbsp;title  = {{The API Traffic Research Dataset Framework (ATRDF)}},<br>
&nbsp;&nbsp;url    = {https://github.com/ArielCyber/Cisco_Ariel_Uni_API_security_challenge},<br>
&nbsp;&nbsp;year   = {2023}<br>
}
    </div>

    <p style="font-size:.78rem; margin-top:1rem; color:var(--global-text-color-light);">
      Also used in:
      <a href="https://doi.org/10.1016/j.cose.2024.104249" target="_blank">
        Aharon, Dubin, Dvir &amp; Hajaj — <em>Computers &amp; Security</em>, 2025
      </a>
    </p>

  </div><!-- end card -->

</div>
