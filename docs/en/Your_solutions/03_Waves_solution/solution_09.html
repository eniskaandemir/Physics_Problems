<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Damped Harmonic Oscillator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
      background: #f7f7f7;
      color: #222;
    }
    h1, h2 {
      margin-bottom: 0.4rem;
    }
    .controls, .info, .layout {
      background: white;
      border-radius: 12px;
      padding: 16px;
      margin-bottom: 16px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.08);
    }
    .row {
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
      align-items: center;
      margin-bottom: 12px;
    }
    .layout {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 16px;
    }
    canvas {
      width: 100%;
      height: 280px;
      background: #fff;
      border: 1px solid #ddd;
      border-radius: 8px;
    }
    code {
      background: #eee;
      padding: 2px 6px;
      border-radius: 4px;
    }
    input[type="range"] {
      width: 280px;
    }
    .small {
      font-size: 0.95rem;
      line-height: 1.5;
    }
  </style>
</head>
<body>
  <h1>Damped Harmonic Oscillator</h1>

  <div class="controls">
    <div class="row">
      <label for="bSlider"><strong>Damping coefficient b:</strong></label>
      <input id="bSlider" type="range" min="0" max="20" step="0.01" value="2" />
      <span id="bValue">2.00</span>
    </div>

    <div class="row">
      <label for="mInput">m</label>
      <input id="mInput" type="number" step="0.1" value="1.0" />
      <label for="kInput">k</label>
      <input id="kInput" type="number" step="0.1" value="9.0" />
      <label for="x0Input">x(0)</label>
      <input id="x0Input" type="number" step="0.1" value="1.0" />
      <label for="v0Input">v(0)</label>
      <input id="v0Input" type="number" step="0.1" value="0.0" />
      <button id="resetBtn">Reset</button>
    </div>
  </div>

  <div class="info small">
    <h2>Theory</h2>
    <p>The damped oscillator is governed by <code>m x'' + b x' + k x = 0</code>.</p>
    <p>Classification:</p>
    <ul>
      <li><strong>Underdamped:</strong> <code>b^2 &lt; 4mk</code></li>
      <li><strong>Critically damped:</strong> <code>b^2 = 4mk</code></li>
      <li><strong>Overdamped:</strong> <code>b^2 &gt; 4mk</code></li>
    </ul>
    <p id="classification"></p>
    <p>This simulation uses the RK4 method to solve the system numerically.</p>
  </div>

  <div class="layout">
    <div>
      <h2>x(t)</h2>
      <canvas id="xtCanvas" width="700" height="280"></canvas>
    </div>
    <div>
      <h2>Phase Portrait</h2>
      <canvas id="phaseCanvas" width="700" height="280"></canvas>
    </div>
  </div>

  <script>
    const bSlider = document.getElementById("bSlider");
    const bValue = document.getElementById("bValue");
    const mInput = document.getElementById("mInput");
    const kInput = document.getElementById("kInput");
    const x0Input = document.getElementById("x0Input");
    const v0Input = document.getElementById("v0Input");
    const resetBtn = document.getElementById("resetBtn");
    const classification = document.getElementById("classification");

    const xtCanvas = document.getElementById("xtCanvas");
    const phaseCanvas = document.getElementById("phaseCanvas");
    const xtCtx = xtCanvas.getContext("2d");
    const phaseCtx = phaseCanvas.getContext("2d");

    function derivatives(state, t, m, b, k) {
      const [x, v] = state;
      const dxdt = v;
      const dvdt = -(b / m) * v - (k / m) * x;
      return [dxdt, dvdt];
    }

    function rk4Step(state, t, dt, m, b, k) {
      const k1 = derivatives(state, t, m, b, k);
      const s2 = [state[0] + 0.5 * dt * k1[0], state[1] + 0.5 * dt * k1[1]];
      const k2 = derivatives(s2, t + 0.5 * dt, m, b, k);
      const s3 = [state[0] + 0.5 * dt * k2[0], state[1] + 0.5 * dt * k2[1]];
      const k3 = derivatives(s3, t + 0.5 * dt, m, b, k);
      const s4 = [state[0] + dt * k3[0], state[1] + dt * k3[1]];
      const k4 = derivatives(s4, t + dt, m, b, k);

      return [
        state[0] + (dt / 6) * (k1[0] + 2 * k2[0] + 2 * k3[0] + k4[0]),
        state[1] + (dt / 6) * (k1[1] + 2 * k2[1] + 2 * k3[1] + k4[1])
      ];
    }

    function simulate() {
      const m = parseFloat(mInput.value);
      const b = parseFloat(bSlider.value);
      const k = parseFloat(kInput.value);
      const x0 = parseFloat(x0Input.value);
      const v0 = parseFloat(v0Input.value);

      const disc = b * b - 4 * m * k;
      let label = "";
      if (Math.abs(disc) < 1e-6) label = "Critically damped";
      else if (disc < 0) label = "Underdamped";
      else label = "Overdamped";

      classification.textContent = `Current regime: ${label} because b² - 4mk = ${disc.toFixed(3)}.`;
      bValue.textContent = b.toFixed(2);

      const tMax = 10;
      const dt = 0.01;
      const points = [];
      let state = [x0, v0];
      let t = 0;

      while (t <= tMax) {
        points.push({ t, x: state[0], v: state[1] });
        state = rk4Step(state, t, dt, m, b, k);
        t += dt;
      }

      drawXT(points);
      drawPhase(points);
    }

    function clearCanvas(ctx, canvas) {
      ctx.clearRect(0, 0, canvas.width, canvas.height);
      ctx.fillStyle = "#ffffff";
      ctx.fillRect(0, 0, canvas.width, canvas.height);
    }

    function drawAxes(ctx, canvas, xLabel, yLabel) {
      ctx.strokeStyle = "#999";
      ctx.lineWidth = 1;
      ctx.beginPath();
      ctx.moveTo(50, 10);
      ctx.lineTo(50, canvas.height - 30);
      ctx.lineTo(canvas.width - 10, canvas.height - 30);
      ctx.stroke();

      ctx.fillStyle = "#333";
      ctx.font = "14px Arial";
      ctx.fillText(yLabel, 15, 20);
      ctx.fillText(xLabel, canvas.width - 30, canvas.height - 8);
    }

    function drawXT(points) {
      clearCanvas(xtCtx, xtCanvas);
      drawAxes(xtCtx, xtCanvas, "t", "x");

      const tMin = 0;
      const tMax = points[points.length - 1].t;
      let xMin = Math.min(...points.map(p => p.x));
      let xMax = Math.max(...points.map(p => p.x));

      if (Math.abs(xMax - xMin) < 1e-9) {
        xMax += 1;
        xMin -= 1;
      }

      const mapX = t => 50 + (t - tMin) / (tMax - tMin) * (xtCanvas.width - 70);
      const mapY = x => (xtCanvas.height - 30) - (x - xMin) / (xMax - xMin) * (xtCanvas.height - 50);

      xtCtx.strokeStyle = "#1f77b4";
      xtCtx.lineWidth = 2;
      xtCtx.beginPath();

      points.forEach((p, i) => {
        const px = mapX(p.t);
        const py = mapY(p.x);
        if (i === 0) xtCtx.moveTo(px, py);
        else xtCtx.lineTo(px, py);
      });

      xtCtx.stroke();
    }

    function drawPhase(points) {
      clearCanvas(phaseCtx, phaseCanvas);
      drawAxes(phaseCtx, phaseCanvas, "x", "v");

      let xMin = Math.min(...points.map(p => p.x));
      let xMax = Math.max(...points.map(p => p.x));
      let vMin = Math.min(...points.map(p => p.v));
      let vMax = Math.max(...points.map(p => p.v));

      if (Math.abs(xMax - xMin) < 1e-9) {
        xMax += 1;
        xMin -= 1;
      }
      if (Math.abs(vMax - vMin) < 1e-9) {
        vMax += 1;
        vMin -= 1;
      }

      const mapX = x => 50 + (x - xMin) / (xMax - xMin) * (phaseCanvas.width - 70);
      const mapY = v => (phaseCanvas.height - 30) - (v - vMin) / (vMax - vMin) * (phaseCanvas.height - 50);

      phaseCtx.strokeStyle = "#d62728";
      phaseCtx.lineWidth = 2;
      phaseCtx.beginPath();

      points.forEach((p, i) => {
        const px = mapX(p.x);
        const py = mapY(p.v);
        if (i === 0) phaseCtx.moveTo(px, py);
        else phaseCtx.lineTo(px, py);
      });

      phaseCtx.stroke();
    }

    [bSlider, mInput, kInput, x0Input, v0Input].forEach(el => {
      el.addEventListener("input", simulate);
    });

    resetBtn.addEventListener("click", () => {
      bSlider.value = 2;
      mInput.value = 1.0;
      kInput.value = 9.0;
      x0Input.value = 1.0;
      v0Input.value = 0.0;
      simulate();
    });

    simulate();
  </script>
</body>
</html>