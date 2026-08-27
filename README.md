# Bootstrapping

If we want to compare two call center models, Apollo 1 and Apollo 2, we can take
the average call time under each and put the two numbers next to each other.

They will never come out identical. What I actually want to know is whether the
difference between them is real, or whether it would come out differently if we
collected the calls again.

So I resample the calls I already have, with replacement, and recompute the mean
each time. A few thousand rounds later I have a distribution rather than a single
number, and I can see how much that average moves around.

The interval is the part I read, not the point estimate. If the interval for the
difference still covers zero, I have not shown anything, and I would not ask
anyone to ship on it.

Bootstrapping suits this because it does not care what shape the data is in.
Nothing to assume about normality, no test to choose between.

The call times are generated, so this shows the method rather than measuring
anything real.

## Files

- `bootstrapping.ipynb`: the analysis and the plots
- `code`: the same thing as a plain Python script

## Running it

```sh
pip install pandas numpy matplotlib seaborn
python code
```

The notebook additionally uses `ptitprince` for the raincloud plots.

Write-up: <https://endersari.com/projects/bootstrapping/>
