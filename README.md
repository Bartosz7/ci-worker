# CI worker for the OpenCS ontology

The recommended way to use this is via the provided Docker image. Just run:
`docker run -it --rm ghcr.io/opencs-ontology/ci-worker:main python <script name.py> <args>`

## Scripts
- `split_concepts.py` – processes an RDF dump of the core ontology, splits it into individual concept files, and formats them nicely. Args:
  - input file
  - output dir (no trailing slash)
  - whether to fix DBpedia IRIs (0/1) – use when importing broken MAKG dumps
