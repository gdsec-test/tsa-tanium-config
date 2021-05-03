# How to generate Mermaid diagrams
Mermaid is a programmatic visualization engine that renders diagrams and flowcharts written in markdown-like langauge.

This document describes the use of [mermaid-cli](https://github.com/mermaid-js/mermaid-cli) to render mermaid diagrams.

## mermaid-cli
The comamnds below render [tanium-architecture-prod-us.mmd](/docs/diagrams/src/tanium-architecture-prod-us.mmd) in PNG and SVG using the mermaid-cli Docker image.

Replace ```/mnt/c/Repos/gdcorp-infosec/tsa-tanium-config``` with the path to your copy of the repo.
### PNG
```
docker run --rm -it -v /mnt/c/Repos/gdcorp-infosec/tsa-tanium-config/docs/diagrams/:/data minlag/mermaid-cli -i /data/src/tanium-architecture-prod-us.mmd -o /data/res/tanium-architecture-prod-us.png -t default -b white -w 1920
```

### SVG
```
docker run --rm -it -v /mnt/c/Repos/gdcorp-infosec/tsa-tanium-config/docs/diagrams/:/data minlag/mermaid-cli -i /data/src/tanium-architecture-prod-us.mmd -o /data/res/tanium-architecture-prod-us.svg -t default -b white -w 1920 -c /data/src/mermaid-config.json
```
The use of [mermaid-config.json](/docs/diagrams/src/mermaid-config.json) is required for SVG due to <a href="https://github.com/mermaid-js/mermaid/issues/1766">Issue #1766 · mermaid-js/mermaid (github.com)</a>.

## Mermaid Live Editor
For a faster, browser-based method:
* Copy the text from the desired ```.mmd``` file into [Mermaid Live Editor](https://mermaid-js.github.io/mermaid-live-editor) on github.io.
* Download SVG/PNG files directly from the editor's output.
* Manually upload the output files to this GitHub repo, replacing the existing versions.