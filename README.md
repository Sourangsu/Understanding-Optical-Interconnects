# Article 2: SerDes and the electrical channel

One Jupyter notebook reproduces the calculations and numerical plots supporting
*Understanding Optical Interconnects: SerDes and the Electrical Channel*.

## Run locally

1. Save the notebook in a writable folder, or extract this package.
2. Open it in your existing Jupyter environment with a Python kernel.
3. Use **Restart Kernel and Run All Cells**.
4. Check inline plots and the automatically created `article2_outputs/` folder.

The standalone notebook does not require any original PDF, DOCX, image, or section notebook.
It does not download data or install packages while running.

For a new environment:

```bash
python -m pip install -r requirements.txt
python -m jupyterlab
```

Inside an existing notebook environment, `%pip install numpy matplotlib` installs the required
numerical libraries into the active kernel. Numba is optional (`%pip install numba`); without it,
the same DFE algorithm runs in pure Python. No fixed run-time estimate is assumed.

## Outputs

- `figures/`: four numerical plots, each in PNG and SVG format.
- `tables/`: CSV calculations, histogram bins, frequency-response profiles, and BER counts.
- `article2_run_summary.json`: parameters, results, file list, and baseline verification.
- `runtime_versions.json`: actual versions used for this run.
