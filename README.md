# Open-Meteo Hourly Weather Forecast TRMNL Plugin

![preview full](assets/preview_full.png)

Inspired by the stock Weather App on IOS. Using Open-Meteo backend, no API key needed.
Using [beautiful SVG icons by basmilius](https://github.com/basmilius/weather-icons), forked and
then hosted on GitHub Pages [here](https://github.com/andi4000/weather-icons).

Open-Meteo API Documentation: https://open-meteo.com/en/docs

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

Will soon be available as Recipe!

<details>
<summary>Manual Installation</summary>

1. Download plugin zip file from [release page](https://github.com/andi4000/trmnl-open-meteo-weather-forecast/releases)
1. Import zip file into your TRMNL Private Plugin (Plugins > Private Plugin > Import New)
1. Enter the Latitude and Longitude of your location
1. Configure other fields as needed
1. **NOTE**: if you see "Liquid error" messages on display, it is because TRMNL server hasn't fetched the weather data yet. Wait a few minutes or force update via link on the sidebar.
1. ?
1. Profit
</details>

## Known Issues
#### Weather icon, i.e. `weather_code` for daily forecast (today and tomorrow) is wild
> Is there a special reason behind showing the worst case weathercode in daily values?

> Well... simplicity ;-) It also has more issues like precipitation at night and sunny throughout the day.

Upstream issue: open-meteo/open-meteo#228

Ideas for a fix: andi4000/trmnl-open-meteo-weather-forecast#1


## Development
Requires docker.

```bash
cp .trmnlp.yml.sample .trmnlp.yml
# edit the file accordingly, then

./bin/trmnlp
```

### Release
Commits should conform to [Conventional Commits](https://www.conventionalcommits.org). 
GitHub Action will automatically create Release PR, changelog, and bump version accordingly.
When release is ready, simply merge the PR.

## Acknowledgements
- [@usetrmnl](https://github.com/usetrmnl) for the great product! I've been thinking of building one myself from scratch, but never had the time. Definitely not an impulse purchase but it's worth it!
- [usetrmnl/trmnlp](https://github.com/usetrmnl/trmnlp) for great software that makes it easy to develop plugin locally!
