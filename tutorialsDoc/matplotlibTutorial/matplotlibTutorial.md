# Matplotlib tutorial

1. Figure(window, jupyter widgets, etc)
2. Each figure contains one or more Axes
3. Axes: an area where the points can be specified in terms of x-y coordinates.(a plot object). Each Axes contains only one Figure. An Axes contains 2 or 3 (for 3-D image) Axis objects.
4. `Axes` is different from `Axis`
5. `fig = plt.figure` :create an empty figure with no Axes
6. `fig, ax = plt.subplots()`: a figure with a single Axes
7. `fig, axs = plt.subplots(2,2)`: a figure with 2\*2 grid of Axes
8. Interactive matplotlib (plt.ion(), plt.plot([0.1,0.1]))
9. Non-interactive ploting
