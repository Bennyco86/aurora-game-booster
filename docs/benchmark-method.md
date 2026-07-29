# Aurora Benchmark Method

Use repeatable measurements to determine whether an optimization helps a specific
PC and game. Do not compare different scenes, graphics settings, drivers, or thermal
states.

## Record the test system

- Windows edition, version, and build.
- CPU, GPU, RAM capacity/speed, storage, and display refresh rate.
- GPU driver version.
- Game version, resolution, renderer, graphics preset, and frame cap.
- Aurora version and the exact changes applied.

## Test sequence

1. Restart Windows and wait for startup activity to settle.
2. Close unrelated apps and keep the same required background apps for every run.
3. Capture a baseline using the same built-in benchmark or repeatable game route.
4. Run at least three baseline passes.
5. Apply one clearly documented group of changes and restart if required.
6. Repeat the same benchmark at least three times.
7. Compare medians rather than selecting the best run.
8. Use Aurora undo, restart, and repeat when practical to check whether the result is
   reproducible.

## Report

- Average FPS.
- 1% low FPS.
- Frame-time graph or percentile data when available.
- CPU/GPU temperature and utilization.
- Any stutter, crash, visual-quality, latency, or power/noise tradeoff.

Do not claim a universal improvement from one PC, one game, or one unusually good
run. Publish neutral or negative results as well as improvements.

