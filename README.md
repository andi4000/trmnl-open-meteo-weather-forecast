# Open-Meteo Weather Forecast TRMNL Plugin

![preview full](assets/preview_full.png)

Inspired by the stock Weather App on IOS. Using Open-Meteo backend, no API key needed.
Using [beautiful SVG icons by basmilius](https://github.com/basmilius/weather-icons), forked and
then hosted on GitHub Pages [here](https://github.com/andi4000/weather-icons).

Mapping between (WMO) weather code to icon and multi-language description is provided by this
GitHub project: https://github.com/andi4000/weather-app-assets
The first draft was generated with AI help, so it might not be 100% accurate. PRs are welcome :)

## Other Formats
<details>
<summary>Half Horizontal</summary>
![half horizontal](assets/preview_half_horizontal.png)
</details>

<details>
<summary>Half Vertical</summary>
![half vertical](assets/preview_half_vertical.png)
</details>

<details>
<summary>Quadrant</summary>
![quadrant](assets/preview_quadrant.png)
</details>

## Usage
TODO

## Development
Requires docker.

```bash
cp .trmnlp.yml.sample .trmnlp.yml
# edit the file accordingly
./bin/trmnlp
```
