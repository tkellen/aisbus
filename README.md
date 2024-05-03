# aisbus
> Fetch AIS data from one provider and push it to another.

## What is this?
I live on a 12m Grainger TR-40 Trimaran called Yana. The location of this vessel is known in close-to-real time anywhere in the world through [AIS](https://en.wikipedia.org/wiki/Automatic_identification_system). This tool runs in the cloud and pulls the boat's position from APIs that have access to global AIS satellite data. Currently, I use it to push updates for [my boat's position on the app/website noforeignland.com](https://noforeignland.com/boat/yana).

## Development Setup
1. Install [golang 1.22+](https://go.dev/).
2. Install staticcheck `go install honnef.co/go/tools/cmd/staticcheck@latest`.
3. Run `make` to build the application.
4. Copy `.envtemplate` to `.env` and populate the values.
5. Run `make run` to run the application.