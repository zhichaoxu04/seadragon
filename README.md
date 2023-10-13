# seadragon


### Access the cluster
- VPN or VX Remote (Desktop or web-based)
- Windows (X-Win32)
  - Connection Name: seadragon
  - Host: seadragon
  - Login: user
- Macintosh (Native Terminal)
  ```bash
  ssh seadragon -Y user@mdanderson.org
  ```

### Use R-studio in the web
RStudio has been installed as a container on Seadragon. This particular container requires some special work, so a submission script is provided to submit the job. First, submit a job to initial the rstudio:
```bash
module load rstudio-sing/4.2.0
# Modify the job submission .lsf script 
bsub < /rsrch3/home/department/user/rserver_4.2.0.lsf
# Use bpeek <jobid> to retrieve information
bpeek [jobID] 
```
Login with PuTTY, but first make sure that X11 forwarding has been enabled:
```bash
# Host Name in the main PuTTY Configuration window
user@mdanderson.org
# Source port
8787
# Destination
edragon023.cm.cluster:12345
```

