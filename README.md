# Moon - Topography grid at 10 arc-minute resolution

Global 10 arc-minute resolution grid of lunar topography referenced to the Lunar
spheroid of [Wieczorek (2015)](https://doi.org/10.1016/b978-0-444-53802-4.00169-x).

![Map of topography showing many circular patterns of both low and high altitude.](preview.jpg)

| | Summary |
|--:|:--|
| File | `moon-topography-10arcmin.nc` |
| Size | 3 Mb |
| Version | [v1](https://github.com/fatiando-data/moon-topography-10arcmin/releases/latest) |
| DOI | https://doi.org/10.5281/zenodo.10693930 |
| License | [CC-BY](https://creativecommons.org/licenses/by/4.0/) |
| MD5 | `md5:0af3363529eb38bb8bbc144c5d756dd9` |
| SHA256 | `sha256:9190261690005fac8d63ed65133e7ab6f691b481a0bd6f52bcfb907b5dfadda2` |
| Source |  Wieczorek, M. A. (2015). Spherical harmonic model of the shape of Earth's Moon: MoonTopo2600p [Data set]. Zenodo. doi:[10.5281/zenodo.3870924](https://doi.org/10.5281/zenodo.3870924) |
| Original license | [CC-BY](https://doi.org/10.5281/zenodo.3870924) |
| Processing code | [`prepare.ipynb`](https://nbviewer.org/github/fatiando-data/moon-topography-10arcmin/blob/main/prepare.ipynb) |

## Changes made

> These are the changes made to the original dataset.

* Expand the spherical harmonic model into a grid.
* Convert the radius data into topography by subtracting the radius of the
  lunar reference sphere of
  [Wieczorek (2015)](https://doi.org/10.1016/b978-0-444-53802-4.00169-x).

## About this repository

This is a place to format and prepare the original dataset for use in our
tutorials and documentation.

We include the source code that prepares the datasets for redistribution by
filtering, standardizing, converting coordinates, compressing, etc.
The goal is to make loading the data as easy as possible (e.g., a single call
to `pandas.read_csv` or `xarray.load_dataset`).
Whenever possible, the code also downloads the original data (otherwise the
original data are included in this repository).

> 💡 **Tip:** The easiest way to download this dataset is using
> [Pooch](https://www.fatiando.org/pooch), particularly to download straight
> from the DOI of a release.

## Contributing

See our [Contributing Guidelines][contrib] for information on proposing new
datasets and making changes to this repository.

## License

All Python source code is made available under the BSD 3-clause license. You
can freely use and modify the code, without warranty, so long as you provide
attribution to the authors.

Unless otherwise specified, all data files and figures created by the code are
available under the Creative Commons Attribution 4.0 License (CC-BY).

See [`LICENSE.txt`](LICENSE.txt) for the full text of each license.

The license for the original data is specified in this `README.md` file.


[contrib]: https://github.com/fatiando-data/.github/blob/main/CONTRIBUTING.md
