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
  <h2 style="font-size:1.3rem; font-weight:600; margin-bottom:1.2rem; letter-spacing:.04em;">
    Research Focus Areas
  </h2>

  <!-- Topic Cards -->
  <div class="research-topics-grid" style="display:grid; grid-template-columns:repeat(auto-fit,minmax(170px,1fr)); gap:1rem; margin-bottom:2rem;">

    <div class="topic-card" style="background:linear-gradient(135deg,#0f2027,#203a43,#2c5364); color:#fff; border-radius:12px; padding:1.1rem; text-align:center; box-shadow:0 4px 15px rgba(0,0,0,.25);">
      <div style="font-size:1.8rem; margin-bottom:.4rem;">🤖</div>
      <div style="font-weight:700; font-size:.85rem; letter-spacing:.03em;">AI Model Security</div>
      <div style="font-size:.75rem; opacity:.8; margin-top:.3rem;">SafePickle · NeuPerm · MTD · CDR</div>
      <div style="margin-top:.6rem; font-size:.72rem; background:rgba(255,255,255,.15); border-radius:20px; padding:.2rem .6rem; display:inline-block;">8 papers</div>
    </div>

    <div class="topic-card" style="background:linear-gradient(135deg,#1a1a2e,#16213e,#0f3460); color:#fff; border-radius:12px; padding:1.1rem; text-align:center; box-shadow:0 4px 15px rgba(0,0,0,.25);">
      <div style="font-size:1.8rem; margin-bottom:.4rem;">🔒</div>
      <div style="font-weight:700; font-size:.85rem; letter-spacing:.03em;">Encrypted Traffic</div>
      <div style="font-size:.75rem; opacity:.8; margin-top:.3rem;">TLS · HTTPS · QUIC · Post-Quantum</div>
      <div style="margin-top:.6rem; font-size:.72rem; background:rgba(255,255,255,.15); border-radius:20px; padding:.2rem .6rem; display:inline-block;">11 papers</div>
    </div>

    <div class="topic-card" style="background:linear-gradient(135deg,#0d0d0d,#1a1a2e,#2d1b69); color:#fff; border-radius:12px; padding:1.1rem; text-align:center; box-shadow:0 4px 15px rgba(0,0,0,.25);">
      <div style="font-size:1.8rem; margin-bottom:.4rem;">🔑</div>
      <div style="font-weight:700; font-size:.85rem; letter-spacing:.03em;">API Security</div>
      <div style="font-size:.75rem; opacity:.8; margin-top:.3rem;">Few-Shot Detection · Injection</div>
      <div style="margin-top:.6rem; font-size:.72rem; background:rgba(255,255,255,.15); border-radius:20px; padding:.2rem .6rem; display:inline-block;">2 papers</div>
    </div>

    <div class="topic-card" style="background:linear-gradient(135deg,#0f2027,#1c4a3f,#2d6a4f); color:#fff; border-radius:12px; padding:1.1rem; text-align:center; box-shadow:0 4px 15px rgba(0,0,0,.25);">
      <div style="font-size:1.8rem; margin-bottom:.4rem;">🛡️</div>
      <div style="font-weight:700; font-size:.85rem; letter-spacing:.03em;">CDR</div>
      <div style="font-size:.75rem; opacity:.8; margin-top:.3rem;">PDF · RTF · Image · AI Models</div>
      <div style="margin-top:.6rem; font-size:.72rem; background:rgba(255,255,255,.15); border-radius:20px; padding:.2rem .6rem; display:inline-block;">5 papers</div>
    </div>

    <div class="topic-card" style="background:linear-gradient(135deg,#1a0533,#2d1b69,#4a148c); color:#fff; border-radius:12px; padding:1.1rem; text-align:center; box-shadow:0 4px 15px rgba(0,0,0,.25);">
      <div style="font-size:1.8rem; margin-bottom:.4rem;">📡</div>
      <div style="font-weight:700; font-size:.85rem; letter-spacing:.03em;">Network Anomaly</div>
      <div style="font-size:.75rem; opacity:.8; margin-top:.3rem;">GNN · Cloud · Malware C2</div>
      <div style="margin-top:.6rem; font-size:.72rem; background:rgba(255,255,255,.15); border-radius:20px; padding:.2rem .6rem; display:inline-block;">4 papers</div>
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
