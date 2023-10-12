# seadragon


### Accessing the cluster
- VPN or VX Remote (Desktop or web-based)
- Windows (X-Win32)
- Macintosh (Native Terminal)
  ```bash
  ssh seadragon [-X or -Y]
  ```

### Using R-studio
```bash
module load rstudio-sing/4.2.0
bsub < /rsrch3/home/department/user/rserver_4.2.0.lsf
bpeek [jobID]
```
