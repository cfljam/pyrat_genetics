# pyrat_genetics

- use R genetics tools for Jupyter Notebooks
- also install base BioConductor packages
- add in additional tools by appending to R-requirements.txt

------------------
Run a temporary notebook server on port 8888 of the host with notebooks served
from my home directory on the host

```
docker run -it --rm -p 8888:8888 \
  -v /Users/johnmccallum/:/HOME cfljam/pyrat_genetics \
  sh -c "ipython notebook --ip=0.0.0.0 \
  --port=8888 --no-browser --notebook-dir=/HOME"
```
