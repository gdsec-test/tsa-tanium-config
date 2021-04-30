# How to generate Mermaid diagrams
Mermaid is a programmatic visualization engine that renders diagrams and flowcharts written in markdown-like langauge.

This document describes the use of [mermaid-cli](https://github.com/mermaid-js/mermaid-cli) to render mermaid diagrams.

## Examples
The comamnds below render [tanium-architecture-prod-us.mmd](/docs/diagrams/src/tanium-architecture-prod-us.mmd) in PNG and SVG using the mermaid-cli Docker image:

### PNG
```
docker run -it -v ~/gdcorp-infosec/tsa-tanium-config/docs/diagrams/:/data minlag/mermaid-cli -i /data/src/tanium-architecture-prod-us.mmd -o /data/res/tanium-architecture-prod-us.png
```

### SVG
```
docker run -it -v ~/gdcorp-infosec/tsa-tanium-config/docs/diagrams/:/data minlag/mermaid-cli -i /data/src/tanium-architecture-prod-us.mmd -o /data/res/tanium-architecture-prod-us.svg -t default -b white -w 1280 -c /data/src/mermaid-config.json
```
The use of [mermaid-config.json](/docs/diagrams/src/mermaid-config.json) is required for SVG due to <a href="https://github.com/mermaid-js/mermaid/issues/1766">Issue #1766 · mermaid-js/mermaid (github.com)</a>.
