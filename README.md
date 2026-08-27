# Bootstrapping

If we want to compare two call center models, Apollo 1 and Apollo 2, we can take
the average call time under each and see which one is lower.

My question here is not which mean is lower. It is whether there is a real
difference if we collect the calls again.

So I resample the observed calls with replacement, recompute the mean each time,
and end up with a distribution for each model instead of a single number.
Bootstrapping assumes nothing about the shape of the data, which is the reason to
reach for it.

What I read off the result is the interval, not the point estimate. If the
interval for the difference between the two models contains zero, then the gap in
the raw means is not something I would act on.

The call times are generated, so the numbers here demonstrate the method rather
than measure anything.

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
