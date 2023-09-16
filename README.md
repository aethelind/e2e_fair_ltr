
# End-to-End Learning for Fair Ranking Systems

Learning to rank subject to constraints on group exposure, using differentiable optimization modules in predict-and-optimize fashion.

See the accompanying paper in WWW '22: <https://arxiv.org/abs/2111.10723>

Required datasets for this project can be found by following the instructions on <https://github.com/him229/fultr>

Credit to the original authors Himank Yadav et. al. for the LTR data and several code segments

For an example command to run the main program, see main.sh

## Notes

- created `requirements.txt` so i can run it locally `pipreqs . --force` then `pip install -r requirements.txt`
- running main with `sh main.sh` is busted, use `source main.sh` instead for the conda command
  - but the conda command `Could not find conda environment: fair_ltr_testing` anyway sooo
- ``np.float` was a deprecated alias for the builtin `float`. To avoid this error in existing code, use `float` by itself.`
  - replaces `np.float` with `float`
- dependency on `https://github.com/JayMan91/NeurIPSIntopt`
- data:
  - originals:
    - We use MSLR and German Credit Datasets for training. They can be found online using the links below:
    - MSLR-WEB30K (Fold 1) - https://www.microsoft.com/en-us/research/project/mslr/
    - German Credit - https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data)
  - see `transformed_datasets/readme.md` and download the transformed data from gdrive


