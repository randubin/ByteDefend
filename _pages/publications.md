---
layout: page
permalink: /publications/
title: publications
description: >
  Publications by <strong>Ran Dubin</strong> spanning AI Model Security, Encrypted Traffic Analysis,
  API Security, Content Disarm &amp; Reconstruction, and Network Anomaly Detection.
  <br>Full list on <a href="https://scholar.google.com/citations?user=kHW5Is4AAAAJ" target="_blank">Google Scholar</a>
  &nbsp;|&nbsp; <a href="https://dblp.org/pid/132/7955" target="_blank">DBLP</a>
  &nbsp;|&nbsp; <a href="https://www.linkedin.com/company/108583398/" target="_blank">ByteDefend Lab</a>
years: [2026, 2025, 2024, 2023, 2022, 2020, 2019, 2018, 2017]
nav: true
nav_order: 1
---

<!-- Research Focus Visualization -->
<div class="research-viz-container" style="margin-bottom:3rem;">
  <h2 style="font-size:1.3rem; font-weight:600; margin-bottom:1.2rem; letter-spacing:.04em; color:var(--global-text-color);">
    Research Focus Areas
  </h2>

  <!-- Topic Cards -->
  <div class="research-topics-grid" style="display:grid; grid-template-columns:repeat(auto-fit,minmax(180px,1fr)); gap:1rem; margin-bottom:2rem;">

    <div class="topic-card" style="background:var(--global-bg-color); border:1px solid rgba(14,165,233,.35); border-left:5px solid #0ea5e9; border-radius:10px; padding:1.2rem 1rem; text-align:center; box-shadow:0 2px 10px rgba(0,0,0,.08);">
      <div style="font-size:2rem; margin-bottom:.5rem;">🤖</div>
      <div style="font-weight:800; font-size:.9rem; color:var(--global-text-color); margin-bottom:.35rem;">AI Model Security</div>
      <div style="font-size:.75rem; color:var(--global-text-color-light); line-height:1.5;">SafePickle · NeuPerm · MTD · CDR</div>
      <div style="margin-top:.7rem; font-size:.72rem; font-weight:700; background:#0ea5e9; color:#fff; border-radius:20px; padding:.25rem .7rem; display:inline-block;">8 papers</div>
    </div>

    <div class="topic-card" style="background:var(--global-bg-color); border:1px solid rgba(99,102,241,.35); border-left:5px solid #6366f1; border-radius:10px; padding:1.2rem 1rem; text-align:center; box-shadow:0 2px 10px rgba(0,0,0,.08);">
      <div style="font-size:2rem; margin-bottom:.5rem;">🔒</div>
      <div style="font-weight:800; font-size:.9rem; color:var(--global-text-color); margin-bottom:.35rem;">Encrypted Traffic</div>
      <div style="font-size:.75rem; color:var(--global-text-color-light); line-height:1.5;">TLS · HTTPS · QUIC · Post-Quantum</div>
      <div style="margin-top:.7rem; font-size:.72rem; font-weight:700; background:#6366f1; color:#fff; border-radius:20px; padding:.25rem .7rem; display:inline-block;">11 papers</div>
    </div>

    <div class="topic-card" style="background:var(--global-bg-color); border:1px solid rgba(16,185,129,.35); border-left:5px solid #10b981; border-radius:10px; padding:1.2rem 1rem; text-align:center; box-shadow:0 2px 10px rgba(0,0,0,.08);">
      <div style="font-size:2rem; margin-bottom:.5rem;">🔑</div>
      <div style="font-weight:800; font-size:.9rem; color:var(--global-text-color); margin-bottom:.35rem;">API Security</div>
      <div style="font-size:.75rem; color:var(--global-text-color-light); line-height:1.5;">Few-Shot Detection · Injection</div>
      <div style="margin-top:.7rem; font-size:.72rem; font-weight:700; background:#10b981; color:#fff; border-radius:20px; padding:.25rem .7rem; display:inline-block;">2 papers</div>
    </div>

    <div class="topic-card" style="background:var(--global-bg-color); border:1px solid rgba(245,158,11,.35); border-left:5px solid #f59e0b; border-radius:10px; padding:1.2rem 1rem; text-align:center; box-shadow:0 2px 10px rgba(0,0,0,.08);">
      <div style="font-size:2rem; margin-bottom:.5rem;">🛡️</div>
      <div style="font-weight:800; font-size:.9rem; color:var(--global-text-color); margin-bottom:.35rem;">CDR</div>
      <div style="font-size:.75rem; color:var(--global-text-color-light); line-height:1.5;">PDF · RTF · Image · AI Models</div>
      <div style="margin-top:.7rem; font-size:.72rem; font-weight:700; background:#f59e0b; color:#fff; border-radius:20px; padding:.25rem .7rem; display:inline-block;">5 papers</div>
    </div>

    <div class="topic-card" style="background:var(--global-bg-color); border:1px solid rgba(239,68,68,.35); border-left:5px solid #ef4444; border-radius:10px; padding:1.2rem 1rem; text-align:center; box-shadow:0 2px 10px rgba(0,0,0,.08);">
      <div style="font-size:2rem; margin-bottom:.5rem;">📡</div>
      <div style="font-weight:800; font-size:.9rem; color:var(--global-text-color); margin-bottom:.35rem;">Network Anomaly</div>
      <div style="font-size:.75rem; color:var(--global-text-color-light); line-height:1.5;">GNN · Cloud · Malware C2</div>
      <div style="margin-top:.7rem; font-size:.72rem; font-weight:700; background:#ef4444; color:#fff; border-radius:20px; padding:.25rem .7rem; display:inline-block;">4 papers</div>
    </div>

  </div>

  <!-- Chart.js Radar Chart -->
  <div style="max-width:520px; margin:0 auto;">
    <canvas id="researchRadar" height="300"></canvas>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
<script>
(function() {
  var ctx = document.getElementById('researchRadar');
  if (!ctx) return;
  var isDark = document.documentElement.getAttribute('data-theme') === 'dark'
    || document.body.classList.contains('dark');
  var gridColor = isDark ? 'rgba(255,255,255,0.15)' : 'rgba(0,0,0,0.1)';
  var labelColor = isDark ? '#ccc' : '#444';

  new Chart(ctx, {
    type: 'radar',
    data: {
      labels: [
        'AI Model Security',
        'Encrypted Traffic',
        'API Security',
        'CDR',
        'Network Anomaly'
      ],
      datasets: [{
        label: 'Publication Count',
        data: [8, 11, 2, 5, 4],
        backgroundColor: 'rgba(44, 130, 201, 0.25)',
        borderColor: 'rgba(44, 130, 201, 0.9)',
        borderWidth: 2.5,
        pointBackgroundColor: 'rgba(44, 130, 201, 1)',
        pointRadius: 5,
        pointHoverRadius: 7
      }]
    },
    options: {
      responsive: true,
      plugins: {
        legend: { display: false },
        tooltip: {
          callbacks: {
            label: function(ctx) { return ' ' + ctx.raw + ' publications'; }
          }
        }
      },
      scales: {
        r: {
          min: 0,
          max: 12,
          ticks: { stepSize: 3, color: labelColor, font: { size: 11 } },
          grid: { color: gridColor },
          angleLines: { color: gridColor },
          pointLabels: { color: labelColor, font: { size: 12, weight: '600' } }
        }
      }
    }
  });
})();
</script>

<!-- Publications List -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
