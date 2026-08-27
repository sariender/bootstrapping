# Bootstrapping

If we want to compare two call center models, Apollo 1 and Apollo 2, we can take
the average call time under each and see which one is lower.

My question here is not which mean is lower. It is whether there is a real
difference if we collect the calls again.

Bootstrapping resamples the observed calls with replacement, recomputes the mean
each time, and gives a distribution instead of a single number. It assumes nothing
about the shape of the data, which is the reason to use it.

The call times here are generated, not real data.

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
