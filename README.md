# pangeo_showcase_20221012

Notes: after the presentation, some people were asking whether the recommendation to use 10 dask workers would be optimal.  I discovered that this is actually the recommended best practice from ECMWF!

From: https://confluence.ecmwf.int/display/COPSRV/Best+practices :

> Speed up retrieval through concurrency:
  The CDS enforces a per user limit to the number of requests that can be processed in parallel. This limit is 10 parallel requests running at the same time. The are also 'global limits' that can affect the user requests.   Whilst submitting multiple requests can improve the tasks' index in the queuing system, the user needs to understand that overloading the system with requests will eventually slow down the overall system performance.  Too many parallel requests could eventually result in a slower overall download time.   For this reason we suggest to limit to a maximum of 10 parallel requests.
